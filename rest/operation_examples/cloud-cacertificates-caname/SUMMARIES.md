# Example summary titles — `/cloud/caCertificates/{caname}`

## DELETE request

### `DELETE/request.json`

| Field | Value |
|---|---|
| **Example name** | `request` |
| **Summary title** | `content (full PEM) required to identify the certificate` |

## DELETE response

### `DELETE/success.json`

| Field | Value |
|---|---|
| **Example name** | `success` |
| **Summary title** | `Empty string on success` |
| **HTTP status** | `200` |

Path parameter example: `caname` = `AmazonRootCA1`

## Live test results (30 Aug 2026)

1. **DELETE** — item 1 from the prior "NEED LIVE TEST" note ("name comes from path `{caname}` only, no request body") was **incorrect**. Live MQTT testing confirmed the reader matches the certificate to delete by its `content` (full PEM), not by `name` alone: `{"name": "FXR-Lab-Test-Root-CA"}` and `{"name": "FXR-Lab-Test-Root-CA.crt"}` both failed with `INVALID CA CERTIFICATE NAME`; adding `content` (the same PEM used to install it) succeeded. `content` is now documented as required in `RestDeveloperfile.yaml` and `mqtt/openapi_md.json`. Only tested via MQTT — REST behavior (body `content` alongside path `{caname}`) is inferred from the same underlying implementation, not separately confirmed.
2. **PUT** — still not separately live-tested for the REST-vs-MQTT `name` handling described in the original note.
