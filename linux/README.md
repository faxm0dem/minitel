# minitelws

## Synopsis

```
minitelws ws://go.minipavi.fr:8182' /dev/ttyAMA0 9600 VIDEOTEX
```

Connects serial device to websocket server


## systemd

You can use the unit file description to initiate connection on startup or user login.
The latter can for instance be achieved by copying the unitfile to '/etc/systemd/user/' and enabling it as follows:

```
systemd --user enable --now minitelws
```

## Credits

This is mainly a copy of [cquest/websocket2minitel](https://github.com/cquest/websocket2minitel) with some additions like minitel initialization from [Zigazou/PyMinitel](https://github.com/Zigazou/PyMinitel).

