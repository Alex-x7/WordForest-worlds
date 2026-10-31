# WordForest content storage

Technical storage used by the WordForest application to retrieve versioned content.

- `catalog/index.json`: digitally signed content index.
- Release attachments: encrypted `.wfp` asset packages.

The application verifies the index signature, package size, SHA-256 and AES-256-GCM authentication before storing accepted content locally for offline use.

Application source code, content keys, private signing keys and player data are not stored in this repository.

This repository is public. Package encryption prevents ordinary browsing of the enclosed assets; it does not provide DRM or prevent reverse engineering.

Published package revisions are immutable. Updates use new revision identifiers and a new signed catalog version.
