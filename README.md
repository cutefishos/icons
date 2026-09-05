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
