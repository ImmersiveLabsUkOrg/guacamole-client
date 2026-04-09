# Upstream Changelog: 0537c89 → b4f4a1f (1.6.0 → 1.6.1)

## New Features

| Ticket | Description |
|--------|-------------|
| GUACAMOLE-2130 | **Linked Records support in Keeper Secrets Manager (KSM)** — Adds support for "linked records" in the KSM vault integration |
| GUACAMOLE-2025 | **Close button for recording video player** — Adds a UI button to close the session recording video player |
| GUACAMOLE-2020 | **Hide display statistics bar** — Adds an option to hide the display statistics overlay |
| GUACAMOLE-2080 | **Sequential touch ID mapping** — Automatically maps local touch IDs to predictable, sequential integer IDs for multi-touch support |
| GUACAMOLE-1170 | **Sized IntegerPool for stream index reuse** — Maximizes time between stream index reuse to avoid ambiguity |
| GUACAMOLE-2131 | **Filter API based on existing objects** — API filtering now takes existing objects into account where available |
| GUACAMOLE-2119 | **Docker `_FILE` variable support** — Adds a setting to enable reading `_FILE` environment variables by default in Docker deployments |
| GUACAMOLE-2139 | **Automated build improvements** — Automatic license retrieval, extension compatibility detection, `API_VERSION` and version number management via Maven `revision` property |
| GUACAMOLE-2248 | **ASF YAML configuration** — Adds `.asf.yaml` for repository details and preferences |

## Bug Fixes

| Ticket | Description |
|--------|-------------|
| GUACAMOLE-1972 | Fix writing **UTF-8 strings with surrogate pairs** |
| GUACAMOLE-2217 | Fix **Caps Lock synchronization issues on Mac** |
| GUACAMOLE-1823 | Fix **unreliable Caps Lock behavior on macOS Chrome** (keyup and keydown) |
| GUACAMOLE-2222 | Fix **mouse events not generated** after browser blur & focus (only keyboard events were) |
| GUACAMOLE-2216 | Fix **mouse position not updated** on mousedown/mouseup events |
| GUACAMOLE-2167 | Fix **incorrect handling of the AltGr key** |
| GUACAMOLE-2175 | **Wait for clipboard synchronization** before pasting |
| GUACAMOLE-2147 | Fix **order of keystroke log** in session recordings |
| GUACAMOLE-2069 | Fix **order of select field items** in the UI |
| GUACAMOLE-2043 | Fix **playback of recordings** containing multibyte character instructions (Unicode surrogate pairs) |
| GUACAMOLE-2036 | Fix **GuacamoleParser** to support multibyte characters; increase max instruction elements to match guacamole-server; refactor internal buffer handling |
| GUACAMOLE-2032 | Fix `hasClientGroups()` to **no longer count the currently attached client** |
| GUACAMOLE-2030 | Fix **KSM static token mapping** for per-user vault config; show Keeper notation warning only once |
| GUACAMOLE-2021 | Fix **session recording playback heatmap** for short videos |
| GUACAMOLE-2018 | Fix `exportState()` to **only convert layer to canvas if non-empty** |
| GUACAMOLE-2005 | **Filter out empty keystroke batches** in recordings |
| GUACAMOLE-2003 | Add **missing clipboard UI options for Kubernetes** connections |
| GUACAMOLE-2088 | Fix **typo in MySQL method name** ("case" not "caes"); add missing `AND` in MySQL/MariaDB `DELETE` query |
| GUACAMOLE-2099 | Add missing `AND` in **SQL Server permission deletion** query; fix typos in SQL Server mapper files |
| GUACAMOLE-2212 | **Reload translations on login** (language changes now take effect immediately) |
| GUACAMOLE-2204 | Add **cache-busting query parameters** to JavaScript resources |
| GUACAMOLE-2198 | Add missing **`ERROR_CLIENT_205` translation** for connection resource conflicts |
| GUACAMOLE-2181 | **Logging improvements** — silence noisy WebSocket errors, fix NPE on early shutdown, consistent log format, extension info in log messages, RADIUS log clarity, remove invalid LDAP overlay reference, disable WADL support |

## Security Patches

| Ticket | Description |
|--------|-------------|
| GUACAMOLE-2004 | Fix **KSM integration for RHEL systems with FIPS mode** enabled (manual BouncyCastle FIPS provider loading) |
| GUACAMOLE-2099 | **Update PostgreSQL and MySQL JDBC drivers** to latest versions (addresses known CVEs in older driver versions) |

## Translation Updates

| Ticket | Language |
|--------|----------|
| GUACAMOLE-2194 | Chinese (`zh.json`) — refined translations, SFTP timeout field |
| GUACAMOLE-2173 | Turkish — new strings and typo fixes |
| GUACAMOLE-2125 | Czech — updated translation |
