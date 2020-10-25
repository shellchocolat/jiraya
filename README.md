A tool for interacting with MS605 magnetic stripe reader/writer.  
It works in a console and allows the user to read/write/copy in ISO/RAW mode.

Not well coded, a lot of redondant code ! Take it as is ^^

## COMMAND LINE
```
./jiraya --help
Usage: ./jiraya.py --help

Options:
  -h, --help            show this help message and exit
  -d DEV, --dev=DEV     /dev/ttyUSB0
  -t TYPE, --type=TYPE  <iso,raw>
  -m MODE, --mode=MODE  <hico,loco>
  -c CMD, --cmd=CMD     <read,write,...>
```

example:
Read a RAW card in Lo-Co mode
```
./jiraya -t raw -m loco -c read
```

commands available:
* read, bulk_read
* write, bulk_write
* copy, bulk_copy
* erase, bulk_erase

## CONSOLE MODE
You can also use the tool as a shell
```
./jiraya
```

You also have a help menu.

More, you can easily save your dumps:
* save
* autosave
