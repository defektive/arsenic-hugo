### Default Op README.md

This file should live in `report/sections/README.md` and be symlinked to the op root directory

#### Curious how to get started?

- edit config.toml
- create a scope file
- run some commands
- browse data

```bash
echo example.com > scope-domains.txt
ar-recon-discover-domains
```

```bash
echo 192.168.0.1/24 > scope-ips.txt
ar-recon-discover-ips
```
