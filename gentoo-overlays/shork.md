{{- $calctime := "/assets/helpers/calctime" -}}

| Directory           | Description                                | Last successful sync                                        |
|---------------------|--------------------------------------------|-------------------------------------------------------------|
| `./guru`            | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/guru" "75m"}}        |
| `./hypr`            | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/hypr" "75m"}}        |
| `./kde`             | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/kde" "75m"}}         |
| `./librewolf`       | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/librewolf" "75m"}}   |
| `./melody`          | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/melody" "75m"}}      |
| `./steam`           | Overlay Mirror                             | {{ include $calctime "/gentoo-overlays/steam" "75m"}}       |

<br>

### Usage
Add to `/etc/portage/repos.conf`:

```
[reponame]
location = /var/db/repos/reponame
sync-type = rsync
sync-uri = rsync://mirrors.shork.ch/gentoo-overlays/reponame
```

