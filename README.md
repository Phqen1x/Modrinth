# Modrinth Snap

Snap packaging for the Modrinth App launcher.

## Install

Install directly from the Snap Store:

```
sudo snap install modrinth
```

## Build from source

1. Download the Modrinth App `.deb` and save it as `modrinth-app.deb` in the repository root.
2. Install Snapcraft: `sudo snap install snapcraft --classic`
3. Build the snap (Ubuntu 24.04 host required): `snapcraft pack`
4. Install locally: `sudo snap install --dangerous modrinth_*.snap`

## Data location

All app data and modpack installs are stored under `~/snap/modrinth/common`.
