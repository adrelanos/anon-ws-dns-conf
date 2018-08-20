# DNS configuration Anonymity Linux Distribution Workstations #

Whether a Anonymity Linux Distribution Gateway supports anonymized system DNS
for Workstation's traffic (also known as Transparent DNS Proxy) mainly depends
on the Gateway's firewall.

This package is simply installing /etc/resolv.conf which points to
10.152.152.10, where an Anon-Gateway is supposed to provide a DnsPort on port
53.

When you do not wish to use the Transparent DNS features, this package can be
removed.
## How to install `anon-ws-dns-conf` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org stretch main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-ws-dns-conf`.

```
sudo apt-get install anon-ws-dns-conf
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-ws-dns-conf` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`anon-ws-dns-conf` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
