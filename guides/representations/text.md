---
rank: 6
related_endpoints:
  - get_files_id
related_guides:
  - representations/supported-file-types
required_guides:
  - representations/list-all-representations
  - representations/request-a-representation
  - representations/download-a-representation
alias_paths: []
id: representations/text
cId: representations
scId: null
isIndex: false
---

# Get a text representation

A text representation provides an easy and way to extract plain text
from a document.

Text is generated for all document file types including plain text and
code files supported by Box. This does not include image files as these
do not have a text layer.

Text representations are generated upon upload of the file just like PDFs
and thumbnails.

Text representations are not generated for files larger than 500 megabytes.

## Requesting a text representation

To get a text representation follow the following steps

- [List all representations](./list-all-representations)
- [Request a text representation](./request-a-representation) by passing the
  `X-Ref-Hints`-header with the value `[extracted_text]`.
- [Download the text](./download-a-representation) by calling the
  `url_template`, replacing the `{+asset_path}` with an  empty string.