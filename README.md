# Modrinth Snap

Snap packaging for the Modrinth App launcher.

## Build

1. Download the Modrinth App `.deb` and save it as `modrinth-app.deb` in the repository root.
2. Install Snapcraft: `sudo snap install snapcraft --classic`
3. Build the snap (Ubuntu 24.04 host required): `snapcraft pack`
4. Install locally: `sudo snap install --dangerous modrinth_*.snap`

## Permissions

After installing, connect the additional interfaces used for network monitoring:

```
sudo snap connect modrinth:network-observe
sudo snap connect modrinth:network-manager
```

## Data location

All app data and modpack installs are stored under `~/snap/modrinth/common`.
