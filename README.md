# WIP: Moss Package Recipe for the Heroic Games Launcher

## !!! Note: This is a work in progress as I explore how moss packaging works in AerynOS. However the application does seem to install and function ok !!!

## How to build
Assuming a local repo has been setup (https://aerynos.dev/packaging/workflow/basic-workflow/)

```shell
# Clone the git repo
git clone https://github.com/ChrisArmstrongUK/mosspkg-heroic-games-launcher.git

# Change into the repo directory
cd mosspkg-heroic-games-launcher

# Build the package and move into the local moss repo index
just build
just mv-local

# Sync moss repos and install
moss sync -u
moss install heroic-games-launcher
```