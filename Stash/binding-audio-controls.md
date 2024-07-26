# How to get volume up and volume down keys to work?

## Prerequisites
- [pactl](https://linux.die.net/man/1/pactl)
- [sxhkd](https://github.com/baskerville/sxhkd)

## Configuring it in sxhkd

``` shell
XF86AudioRaiseVolume
    pactl set-sink-volume @DEFAULT_SINK@ +2%

XF86AudioLowerVolume
    pactl set-sink-volume @DEFAULT_SINK@ -2%

XF86AudioMute
    pactl set-sink-mute @DEFAULT_SINK@ toggle
```

