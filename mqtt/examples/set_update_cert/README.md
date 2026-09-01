# `set_update_cert`

REST: `PUT /cloud/certificates` → `cloud-certificates/`

Wire `command` (developer MQTT API): `set_updateCertificate` (alias `set_update_cert`)

Stable `command_id`: `req-set-update-cert`

| File | Direction | Example | REST source | Summary |
|---|---|---|---|---|
| `request/install_certificate_sftp.json` | request | `install_certificate_sftp` | `cloud-certificates/PUT/install_certificate_sftp.json` | Install certificate via SFTP, BASIC auth |
| `request/install_certificate_https_headers.json` | request | `install_certificate_https_headers` | `cloud-certificates/PUT/install_certificate_https_headers.json` | Install certificate over HTTPS with custom headers and retry policy |
| `request/updateCertificate_client.json` | request | `updateCertificate_client` | `cloud-certificates/PUT/updateCertificate_client.json` | Client cert for mTLS MQTT (not yet created) |
| `request/updateCertificate_app.json` | request | `updateCertificate_app` | `cloud-certificates/PUT/updateCertificate_app.json` | App certificate, no download auth (not yet created) |
| `request/updateCertificate_inline_pem.json` | request | `updateCertificate_inline_pem` | `cloud-certificates/PUT/updateCertificate_inline_pem.json` | Inline CA content (not yet created) |
| `response/success.json` | response | `success` | `—` | Command succeeded |

