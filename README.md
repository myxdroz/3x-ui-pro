# 3x-ui-pro

Secure 3x-ui installer for Terramaster F4-425 NAS and other self-hosted setups.

## Quick Start

```bash
curl -sSL https://raw.githubusercontent.com/myxdroz/3x-ui-pro/main/x-ui-latest-v3.10.2.sh | sudo bash -
```

Or download and run:

```bash
wget -qO- https://raw.githubusercontent.com/myxdroz/3x-ui-pro/main/x-ui-latest-v3.10.2.sh | sudo bash
```

## Manual Run

```bash
sudo bash x-ui-latest-v3.10.2.sh \
  -subdomain panel.yourdomain.com \
  -reality_domain reality.yourdomain.com \
  -install y \
  -auto_domain y
```

## Requirements

- Ubuntu 24.04 / 26.04 **or** Debian 12 / 13
- Root access
- Domain with DNS A records pointing to the server IP
- Ports 80, 443 open
- Host-passthrough CPU (not QEMU emulated)

## Supported Features

- Reality + WebSocket + XHTTP + Trojan-gRPC inbounds
- SNI-based stream routing via nginx
- Clash/Mihomo subscription generation
- Network diagnostics page (MTR, speedtest)
- BBR TCP congestion control
- Automatic firewall (UFW)

## License

MIT
