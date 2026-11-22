# Lean Bulk Log: program updates

This repository hosts the program content for the Lean Bulk Log Android app. The app downloads it once a day over HTTPS from GitHub Pages:

    https://maher-elnashrty.github.io/lean-bulk-log-program/program.json

| File | Purpose |
|------|---------|
| `program.json` | Training sessions, foods, menus, targets and tips (English and Arabic) |
| `program.json.sha256` | SHA-256 checksum (integrity) |
| `program.json.sig` | ECDSA P-256 signature (authenticity). The app rejects files not signed with the publisher's key. |

Personal body measurements are deliberately not published. Nutrition and training content is general guidance only, not medical advice.

To publish a new version, run `tools/publish_program.py` in the app project, copy its three output files here, then commit and push.
