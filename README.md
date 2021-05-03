# RebornOS RICE

You can find here some of my early work that I created during ricing of my daily driver [RebornOS](https://rebornos.org/). Repository includes:

1. Grub themes
2. Neofetch logo
3. Wallpapers

Installation procedure for each element below.

## Grub themes:

|Theme 1 (1920x1080)|Theme 2 (1920x1080)|Theme 3 (any resolution)|
|:-:|:-:|:-:|
|![img](https://raw.githubusercontent.com/elkrien/RebornOS-rice/main/theme1.png)|![img](https://raw.githubusercontent.com/elkrien/RebornOS-rice/main/theme2.png)|![img](https://raw.githubusercontent.com/elkrien/RebornOS-rice/main/theme3.png)|

### Installation

##### Copy selected theme folder to :
```shell
/usr/share/grub/themes/
```
##### Edit `/etc/default/grub` to :

For theme 1:
```shell
GRUB_THEME="/usr/share/grub/themes/Grub-theme-1/theme.txt"
```

For theme 2:
```shell
GRUB_THEME="/usr/share/grub/themes/Grub-theme-2/theme.txt"
```

For theme 3:
```shell
GRUB_THEME="/usr/share/grub/themes/Grub-theme-3/theme.txt"
```
##### Optional if You have problems with automatic resolution of grub change line:

```shell
GRUB_GFXMODE=1920x1080
```

(change `1920x1080` to your's screen resolution)

##### Update grub :

```shell
$ sudo grub-mkconfig -o /boot/grub/grub.cfg
```



## Neofetch logo:

Color depends on Your terminal colors:

<img src="https://github.com/elkrien/RebornOS-rice/blob/main/neofetch.png?raw=true"  />

### Installation

##### Copy logo file `rebornos.txt` to :

```shell
~/.config/neofetch
```

##### Edit `~/.config/neofetch/config.conf` to :

```shell
image_source="$HOME/.config/neofetch/rebornos.txt" 
```

##### 