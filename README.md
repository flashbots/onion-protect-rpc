# Onion proxy for rpc.flashbots.net

Stripped down fork of [igor53627/blockscout-onion](https://github.com/igor53627/blockscout-onion)

Serves `http://protectfbnoqyfgo3t5ouw3c7odp55qqoxnfdd7u24nzz5pkbclbzzyd.onion`.

## Setup

1. Install `podman-docker`
2. Drop `tor-ingress.service` to `~/.config/systemd/user/`
3. Build: `docker-compose build`
4. Enable service: `systemctl enable --user --now tor-ingress`
