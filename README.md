# Useful commands

## Wifi connect
```
nmcli —ask device wifi connect <SSID>
```

### Steps
```
install git

clone repo (https)
export NIX_PATH=$PWD
cp harwdare_configuration.nix

sudo nix-channel --add https://github.com/nix-community/home-manager/archive/release-25.05.tar.gz home-manager
sudo nix-channel --update

sudo nixos-rebuild switch -I nixos-config=<CONFIG_PATH>

gh auth login
git set new remote (ssh)
git push …
```

# For kitty in VM
```
LIBGL_ALWAYS_SOFTWARE=1 kitty
```

# For BIOS update
```
fwupdmgr refresh --force
fwupdmgr get-updates
fwupdmgr update
```
