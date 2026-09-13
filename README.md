# nyom dns

[![octodns](https://img.shields.io/github/actions/workflow/status/nyomlol/dns/octodns.yml?branch=main&label=octodns)](https://github.com/nyomlol/dns/actions)
![python](https://img.shields.io/badge/python-3.12-blue)

free nyom.lol subdomains!

## contributing

- fork the repo and add your records to `zones/nyom.lol.yaml`
- run `octodns-format zones/*.yaml` before pushing
- open a pull request

## setup

```bash
pip install -r requirements.txt
```

## commands

| command | description |
| --- | --- |
| `octodns-format zones/*.yaml` | format zone files (run before push) |
| `octodns-format --check zones/*.yaml` | check formatting without modifying |
| `octodns-validate --config-file config.yaml` | validate config and zone data |
| `octodns-sync --config-file config.yaml` | dry-run: preview changes |
| `octodns-sync --config-file config.yaml --doit` | live sync to cloudflare |
