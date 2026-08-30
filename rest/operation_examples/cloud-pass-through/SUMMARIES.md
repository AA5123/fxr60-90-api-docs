# Example summary titles — `/cloud/pass-through`

### `PUT/status.json`

| Field | Value |
|---|---|
| **Example name** | `status` |
| **Summary title** | `RC status command` |

### `PUT/passthru.json`

| Field | Value |
|---|---|
| **Example name** | `passthru` |
| **Summary title** | `RC mode command` |

### `PUT/success.json`

| Field | Value |
|---|---|
| **Example name** | `success` |
| **Summary title** | `RC status reply` |
| **HTTP status** | `200` |
| **Pairs with** | `PUT/status.json` (`payload: status`) |

### `PUT/mode_success.json`

| Field | Value |
|---|---|
| **Example name** | `mode_success` |
| **Summary title** | `RC mode reply` |
| **HTTP status** | `200` |
| **Pairs with** | `PUT/passthru.json` (`payload: mode`) |
