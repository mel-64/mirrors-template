{{- $calctime := "/assets/helpers/calctime" -}}

| Directory           | Description                                | Last successful sync                              |
|---------------------|--------------------------------------------|---------------------------------------------------|
| `/archlinux`        | Package Mirror                             | {{ include $calctime "/archlinux" "60m"}}         |
| `/gentoo`           | Ebuild Mirror                              | {{ include $calctime "/gentoo" "60m" }}           |
| `/gentoo/distfiles` | Distfile Mirror                            | {{ include $calctime "/gentoo/distfiles" "60m"}}  |
| `/termux`           | Package Mirror                             | {{ include $calctime "/termux" "60m" }}           |


