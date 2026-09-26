{{- $calctime := "/assets/helpers/calctime" -}}

| Directory           | Description                                | Last successful sync                              |
|---------------------|--------------------------------------------|---------------------------------------------------|
| `/archlinux`        | Package Mirror                             | {{ include $calctime "/archlinux" "75m"}}         |
| `/gentoo`           | Ebuild Mirror                              | {{ include $calctime "/gentoo" "75m" }}           |
| `/gentoo/distfiles` | Distfile Mirror                            | {{ include $calctime "/gentoo/distfiles" "75m"}}  |
| `/termux`           | Package Mirror                             | {{ include $calctime "/termux" "75m" }}           |


