# kai-dashboard.github.io

Public static pages for the KAI cluster dashboards (off-VPN view).

- **/** → **production** (locust) — data from the production snapshot gist.
- **/workstations/** → **testbed** (the Tailscale workstation mesh) — data from
  the testbed snapshot gist.

Each `index.html` is generated from `BrachioLab/kai-dashboard`
(`python3 dashboard.py --emit-static`) — do not hand-edit. `config.json` in each
directory sets which gist that page reads (`gist_raw_base`). Data is refreshed
~every 5 min by an in-cluster CronJob per cluster; these pages only host the
static UI.
