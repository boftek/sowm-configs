# SOWM

SOWM is one of my preferred window manager in Linux.
\
So I created my owm configs of this WM.
\
Now keep in mind this config is really simple.

### Get SOWM

Clone the repo :)

## Installation

1) You can modify `config.h` to suit your needs.
2) Run `make` to build sowm.
3) Copy it to your path or run `make install`.
    - `DESTDIR` and `PREFIX` are supported.
4) (Optional) Apply patch with `git apply patches/patch-name`
    - In case of applying multiple patches, it has to be done **manually**.

### Launch SOWM (Method 1)
Start `sowm` from `.xinitrc` or use `tty` to start it.

### Lanch SOWM (Method 2)
Launch it using login manager (GDM, LightDM, SDM etc.)
My config includes some functions like autostart. To use them I used this [guide](https://github.com/dylanaraps/sowm/issues/29)
\
In case you want to use mine I included it in folder `sowm-scripts`

## Navigate in SOWM

**Window Managment**

| combo                      | action                 |
| -------------------------- | -----------------------|
| `Mouse`                    | focus under cursor     |
| `MOD4` + `Left Mouse`      | move window            |
| `MOD4` + `Right Mouse`     | resize window          |
| `MOD4` + `f`               | maximize toggle        |
| `MOD4` + `c`               | center window          |
| `MOD4` + `q`               | kill window            |
| `MOD4` + `1-9`             | desktop swap           |
| `MOD4` + `Shift` +`1-9`    | send window to desktop |
| `MOD1` + `TAB` (*alt-tab*) | focus cycle            |

**Programs**

| combo                    | action           | program        |
| ------------------------ | ---------------- | ------------------ |
| `MOD4` + `Return`        | terminal         | `gnome-terminal`   |
| `MOD4` + `d`             | dmenu            | `dmenu_run -h 32`  |
| `MOD4` + `p`             | scrot            | `scr`              |
| `MOD4` + `w`             | wallpaper cycler | `bud`              |
| `XF86_AudioLowerVolume`  | volume down      | `amixer`           |    
| `XF86_AudioRaiseVolume`  | volume up        | `amixer`           |
| `XF86_AudioMute`         | volume toggle    | `amixer`           |
| `XF86_MonBrightnessUp`   | brightness up    | `bri`              |
| `XF86_MonBrightnessDown` | brightness down  | `bri`              |


#### Wallpapers
You can use Nitrogen to change wallpapers. In the `sowm-stuff` I included some beatiful wallpapers by Derek Taylor (DistroTube). Find original repo here [DWT1](https://gitlab.com/dwt1/wallpapers)

#### Additional software
I use sxhkd to do some custom keybinds. \
Nitrogen for setting the wallpapers \
Compton for composting (shadows in terminal etc.) \
Patched dmenu avialiabile [here](https://github.com/philippanic/dotz/tree/master/.config/dmenu)
\
My sxhkd config lives [here](https://github.com/philippanic/dotz/tree/master/.config/sxhkd)


