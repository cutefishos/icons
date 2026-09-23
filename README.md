# Cutefish Icon Theme

Based on [Colloid-icon-theme](https://github.com/vinceliuice/Colloid-icon-theme).

## Build and install

Configure and install the theme with CMake:

```sh
cmake -S . -B build
sudo cmake --install build
```

The default installation directory is `/usr/share/icons`. Set either
`CMAKE_INSTALL_PREFIX` or `INSTALL_PREFIX` to choose another prefix:

```sh
cmake -S . -B build -DCMAKE_INSTALL_PREFIX="$HOME/.local"
cmake --install build
```

The installation provides the `Cutefish` theme under `share/icons`.

The four `src/actions/symbolic/window-*-symbolic.svg` controls are adapted from
FishUI's `src/images/light/` artwork (CutefishOS Team, GPL-3.0-or-later), revision
`4692189f668e0921582337a0b7bdedd4010826c4`. The original paths are translated by
(-4, -4) onto a 16×16 canvas, matching GTK/Chromium's standard icon size without
shrinking the artwork. Symbolic foreground allows GTK recoloring. No custom GTK
CSS is required; select the installed theme with:

```sh
gsettings set org.gnome.desktop.interface icon-theme Cutefish
```
