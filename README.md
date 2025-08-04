# kCraft - Minecraft Launcher

[Kernal](https://kernal.eu/posts/kcraft-minecraft-launcher/) Minecraft Launcher written in bash

# Requirements

 - [jq](https://github.com/stedolan/jq)
 - [aria2](https://github.com/aria2/aria2)
 - [rofi](https://github.com/davatorium/rofi)
 -
# Installation

    install -m 755 kcraft /usr/bin

# Usage

If game version is not provided in arguments then `rofi` selection will spawn. Selected version is then downloaded and run.

```shell
kcraft
```

```shell
kcraft 1.21.7
```

Player name is set to `$USER` by default, can be changed with `--user` option

```shell
kcraft --user Analizer 1.21.7
```

Minecraft files are stored by default in `~/.minecraft`, this can be changed with `--directory` option

```shell
kcraft --directory /mnt/drive1/minecraft 1.21.7
```

If game files become partially corrupted you can redownload them with `--force` option

```shell
kcraft --force 1.21.7
```

You can provide additional arguments for java with `--java-args` option

```shell
kcraft --java-args '-Xmx8G -Xss1M' 1.21.7
```

Get some help

```shell
kcraft -h
```
