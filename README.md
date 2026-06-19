# kai-dashboard.github.io

Public static page for the KAI cluster dashboard (off-VPN view).

- `index.html` — generated from `BrachioLab/kai-dashboard` via
  `python3 dashboard.py --emit-static`. Do not hand-edit.
- `config.json` — points at the snapshot gist (`gist_raw_base`).

Data comes from a gist refreshed every ~5 min by an in-cluster CronJob; this
repo only hosts the (static) page. See BrachioLab/kai-dashboard for the source.
