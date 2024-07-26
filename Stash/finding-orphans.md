# Finding orphan packages in Arch Linux

```shell
pacman -Qtdq # finding
sudo pacman -Rns $(pacman -Qdtq) # uninstalling
```
