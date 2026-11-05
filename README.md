# Modrinth Snap

Snap packaging for the Modrinth App launcher.

## Install

Install directly from the Snap Store:

```
sudo snap install modrinth
```

## Build from source

The snap builds Modrinth App from the [upstream source](https://github.com/modrinth/code) at the tag set by `source-tag` in `snap/snapcraft.yaml`, with the patches in `snap/local/patches` applied.

1. Install Snapcraft: `sudo snap install snapcraft --classic`
2. Build the snap: `snapcraft pack`
3. Install locally: `sudo snap install --dangerous modrinth_*.snap`

## Updates

The in-app updater is disabled, and the snap is updated by snapd. The build leaves out upstream's `updater` Cargo feature, so the updater isn't compiled in.

## Data location

All app data and modpack installs are stored under `~/snap/modrinth/common`.
