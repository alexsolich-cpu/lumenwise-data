# lumenwise-data

The device-identifier file that the LumenWise app fetches between app updates, with the Ed25519 signature the app verifies it against.

Each release holds `device-identifiers.json` (the file, in the app's format) and `device-identifiers.json.sig` (the signature). The app downloads the newest release and uses it in place of the copy bundled with the app. The file holds public catalog data — the same barcodes the app ships with, sourced from the FDA's GUDID, the EU's EUDAMED, manufacturers' ordering tables and boxes read in the lab. The public key is in the [REALIS_LumenWise repository](https://github.com/alexsolich-cpu/REALIS_LumenWise).
