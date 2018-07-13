# bashutils

## watcher

runs the script line in quotes over and over again, producing a chart

usage:
watcher "head /proc/meminfo | grep MemFree | awk '{print int(\$2/4096)}'"

output (ctrl+c to abort)

```sh
watching: head /proc/meminfo | grep MemFree | awk '{print int($2/4096)}'
  128 - -
  127     -
  126       - -
  125  - - -    - - -
  124        -     - ---
  123          - -      --
  122
  121                     -
```
