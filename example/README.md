## Default Op README.md

This file should live in `report/sections/README.md` and be symlinked to the op root directory

### Getting Started

- Update config.toml with desired information

#### Create a Scope

- scope-domains-client-provided.txt
- scope-domains-manually-discovered.txt
- scope-ips-client-provided.txt
- scope-ips-manually-discovered.txt

When running commands typically the glob `scope-domains-*` is used to get a list of domain, and `scope-ips-*` is used to get valid IPs.

#### Discovery Recon

Now we can run `ar-passive-recon`. this will do some basic enumeration about what domains the scope contains and hopefully find some more sub domains.

After we've gathered a list of domains, we can check for SSL certs and see what domains they have using `ar-recon-ssl-certs`.

We should take amoment and add any undesirable domains to `blacklist-domains.txt` and any undesirable IPs to `blacklist-ips.txt`. This will prevent them from being included in most commands...


See [arsenic](https://github.com/defektive/arsenic) for more information
