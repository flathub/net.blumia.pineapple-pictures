# Pineapple Pictures at Flathub

## Info

- Flathub store page: <https://flathub.org/apps/net.blumia.pineapple-pictures>
- Upstream source code: <https://github.com/BLumia/pineapple-pictures/>

## Maintenance Cheatsheet

### Fetch/download dependencies

``` shell
$ flatpak-builder build net.blumia.pineapple-pictures.yml --download-only
```

`tsocks` or similar programs can be used to make `flatpak-builder` go through a proxy.

### (Re)build

``` shell
$ flatpak-builder build net.blumia.pineapple-pictures.yml --force-clean --disable-cache --disable-download
```

### Install to current user

``` shell
$ flatpak-builder build net.blumia.pineapple-pictures.yml --force-clean --disable-download --install --user
```

### Run installed package

``` shell
$ flatpak run net.blumia.pineapple-pictures
```

### Interactive shell for installed flatpak package

```shell
$ flatpak run --command=sh net.blumia.pineapple-pictures
```
