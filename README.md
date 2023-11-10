# How to lauch

First, edit the hardware configuration file to make it work on your current computer.
To generate the default nix configuration, you can use the following command after mounting the partitions:

```sh
sudo nixos-generate-config --root /mnt --show-hardware-config
```

After booting on a nix iso, run the following command :

```sh
nix run --extra-experimental-features nix-command --extra-experimental-features flakes "github:HUB-Lyon/Serveurs#partitioning" --no-write-lock-file
```
