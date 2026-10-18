# Repository compatibility and retention

The canonical public distribution repository is `asygames/asybrain-releases` (GitHub ID **1373532789**, default branch `master`). Its historical name is `asygames/asyindex-releases`.

## Reserved historical name

**Never create another repository named `asygames/asyindex-releases`.** Existing installers, native clients and signed manifests use its GitHub redirect. New publication commands and navigation use the canonical name.

Published Connector 0.2.56 and older clients strictly validate artifact URLs containing the historical repository name. Signed manifest generators intentionally continue emitting that historical artifact prefix until those clients can be retired. New readers accept only the exact canonical repository and the exact historical alias, preserving signature and hash checks. Do not bulk-replace repository names in signed manifests.

## Immutable history

- Preserve historical tags, release IDs, asset IDs, bytes and checksums. Do not overwrite versioned assets, move tags, rewrite Git history or delete old releases as cleanup.
- Stable manifests remain product-specific: `asybrain-connector-stable`, `asybrain-agent-stable`, `asybrain-installer-stable` and legacy `asyremote-stable`. A channel promotion requires its own verified release procedure and rollback copy.
- This rename adds installer 0.1.2 as a separate immutable release. It does not replace existing installer 0.1.1 files or native binaries. The website points to the reviewed version directly; the existing installer stable snapshot is retained.
- AsyIndex Hub is retired by its owner. Preserve all its historical downloads as an archive; its automatic updater is no longer maintained.
- Unrelated repositories such as `asyremote-releases` and `asybrain-hub-releases` retain their own names.

## Verification and catalog maintenance

Compare the GitHub repository ID and every original release/asset ID, name, size and available digest before and after a rename. Verify the old and new API, Git, stable-manifest and asset-download URLs. Validate signed manifests and hash both Windows and Linux binaries.

`CATALOG.md` is a dated inventory grouped by product, not an update manifest. Refresh it from all pages of the GitHub releases API after new publications; do not infer a maintained channel from the newest tag or generic Latest badge. Release history and signed stable manifests remain authoritative.
