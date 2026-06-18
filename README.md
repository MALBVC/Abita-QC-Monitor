# Abita QC Monitor — Dashboard

This repo holds the **generated output** of Abita's QC Monitor dashboard — nothing else.

It is auto-published here after every QC Monitor pipeline run so the Abita brewing team can view current batch status, spec readings, and OOS flags at:

**https://malbvc.github.io/Abita-QC-Monitor/**

There is no application code in this repo. The ingest pipeline, parsers, OOS detection, and database all live in a private repository and run on a separate machine with VPN access to Abita's production network. This repo only ever receives two files:

- `index.html` — the dashboard shell
- `qc-data.js` — the current batch/reading data

Both are overwritten on every publish; there is no commit-by-commit history of meaningful changes, just a rolling snapshot.
