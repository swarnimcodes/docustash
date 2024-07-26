# Finding which installable packages provides a given binary

For instance i needed to find which package provides the binary `pactl`.
In arch linux you can use the following command:

```shell
sudo pacman -Fy pactl
```

Output is like so:

```shell
[swarnim@arch ~]$ sudo !!
sudo pacman -Fy pactl
[sudo] password for swarnim: 
:: Synchronizing package databases...
 core is up to date
 extra is up to date
 multilib is up to date
extra/gstreamer-docs 1.24.5-2
    usr/share/doc/gstreamer/html/assets/js/search/pactl
extra/libpulse 17.0-3 [installed]
    usr/bin/pactl
    usr/share/bash-completion/completions/pactl
```
