{{- $calctime := "/assets/helpers/calctime" -}}

| Directory           | Description                                | Last successful sync                                        |
|---------------------|--------------------------------------------|-------------------------------------------------------------|
| `./guru`            | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/guru" "60m"}}        |
| `./hypr`            | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/hypr" "60m"}}        |
| `./kde`             | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/kde" "60m"}}         |
| `./librewolf`       | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/librewolf" "60m"}}   |
| `./meldoy`          | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/melody" "60m"}}      |
| `./steam`           | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/steam" "60m"}}       |

<br>

### Usage
Add to `/etc/portage/repos.conf`:

```
[reponame]
location = /var/db/repos/reponame
sync-type = rsync
sync-uri = rsync://mirrors.shork.ch/gentoo-overlays/reponame
```

