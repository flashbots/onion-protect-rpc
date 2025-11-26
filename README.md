# Onion proxy for rpc.flashbots.net

Serves `http://protectfbnoqyfgo3t5ouw3c7odp55qqoxnfdd7u24nzz5pkbclbzzyd.onion`.

Stripped down fork of [igor53627/blockscout-onion](https://github.com/igor53627/blockscout-onion), check out its readme for more details.

## Setup

1. Install `podman-docker`
2. Drop `tor-ingress.service` to `~/.config/systemd/user/` (fix paths inside)
3. (optional) Put your `hs_ed25519_*_key` to `tor_data/hidden_service`
3. Build: `docker-compose build`
4. Enable service: `systemctl enable --user --now tor-ingress`
