## Initial
``` bash
brew tap qmk/qmk
brew install qmk

# Need to fork beforehand
qmk setup methodmen/qmk_firmware
qmk compile -kb hhkb -km default
qmk config user.keyboard=hhkb
qmk config user.keymap=methodmen
```

## New keymap
``` bash
qmk new-keymap -kb <keyboard_name>
```
edit keymap.c

## Compile
``` bash
#qmk compile -kb <keyboard> -km default
qmk compile -kb hhkb -km methodmen
```

# Flush
use qmk toolbox. select .build/hhkb_methodmen.hex

