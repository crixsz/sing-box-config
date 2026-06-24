# sing-box Configuration Repository

This repository contains a sample `sing-box` configuration for version **1.13.13**. It is designed to demonstrate a VLESS WebSocket outbound configuration with a TUN inbound interface on Windows.

## Included files

- `README.md` - this documentation file
- `vless-ws-nontls.json` - sample `sing-box` configuration
- `sing-box.exe` - local `sing-box` executable
- `libcronet.dll` - Chromium network library dependency
- `wintun.dll` - Windows TUN driver dependency


## Notes

- This config is targeted for `sing-box` **1.13.13**.
- The TUN inbound requires proper tunneling support on Windows and may need administrator privileges.
- If you only need a proxy client without TUN routing, you can change the inbound type or use a different `sing-box` configuration.

## Customization

- Update DNS servers under `dns.servers` if you want different resolvers.
- Adjust `route.rules` to fit your network requirements.
- Set `multiplex.enabled` to `true` if your server supports multiplexing.

## Disclaimer

This repo is intended as a starting point for `sing-box` users. Verify your server settings and ensure the correct version of `sing-box` is being used before deployment.
