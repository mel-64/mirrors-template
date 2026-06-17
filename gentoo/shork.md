## Merged **Gentoo** Ebuild & Distfile Mirror

### Usage

**Portage ebuild mirror**

Add to `/etc/portage/repos.conf`:

```
[gentoo]
location = /var/db/repos/gentoo
sync-type = rsync
sync-uri = rsync://mirrors.shork.ch/gentoo
```

**Portage distfile mirror**

Add to `/etc/portage/make.conf`:

```
GENTOO_MIRRORS=" \
	rsync://mirrors.shork.ch/gentoo \
	https://mirrors.shork.ch/gentoo \
"
```

