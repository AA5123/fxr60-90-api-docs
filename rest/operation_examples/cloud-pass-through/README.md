# `/cloud/pass-through`

- **PUT** — pass-through command to RC (`component` + `payload`)

## Examples

| File | Direction | Example name | Summary |
|---|---|---|---|
| `PUT/status.json` | request | `status` | RC status command |
| `PUT/passthru.json` | request | `passthru` | RC mode command |
| `PUT/success.json` | response 200 | `success` | RC status reply (pairs with `PUT/status.json`) |
| `PUT/mode_success.json` | response 200 | `mode_success` | RC mode reply (pairs with `PUT/passthru.json`) |
