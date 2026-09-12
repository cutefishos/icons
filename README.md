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

The installation provides `Cutefish`, `Cutefish-Light`, and `Cutefish-Dark`
under `share/icons`.

The four `src/actions/symbolic/window-*-symbolic.svg` controls are adapted from
FishUI's `src/images/light/` artwork (CutefishOS Team, GPL-3.0-or-later), revision
`4692189f668e0921582337a0b7bdedd4010826c4`. Their 24×24 geometry and paths are
unchanged; only the fill is converted to symbolic foreground for GTK recoloring.
