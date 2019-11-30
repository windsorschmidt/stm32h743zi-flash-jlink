## About
Demonstrate flashing STM32H743ZI using J-Link commander.

Tested with J-Link Commander V6.48a.

### Start J-Link Commander

```
root@host# JLinkExe -device STM32H743ZI -if SWD -autoconnect 1 -speed auto
```

### Flash firmware to target
```
J-Link> loadbin nucleo-hz43zi-blinky.bin, 0x8000000
```

### Reset target
```
J-Link> r
J-Link> g
```

### Exit J-Link Commander
```
J-Link> q
```
