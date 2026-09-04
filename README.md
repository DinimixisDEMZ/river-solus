# river-solus

Solus `.eopkg` package for [River](https://codeberg.org/river/river), a non-monolithic Wayland compositor.

## Package

| Package | Description | License | Version |
| :--- | :--- | :---: | :---: |
| [**river**](https://codeberg.org/river/river) | Non-monolithic Wayland compositor | [GPL-3.0-only](https://spdx.org/licenses/GPL-3.0-only.html) | 0.5.0 |

## Installation

Build the package locally with `solbuild`, or download the `.eopkg` from a release.

```bash
sudo eopkg it ./river-0.5.0-1-1-x86_64.eopkg
```

River needs a window manager implementing the `river-window-management-v1` protocol (e.g. `tinyrwm`) and an init script to be useful.

## Building

```bash
cd river
sudo solbuild build package.yml
```

This generates `river-0.5.0-1-1-x86_64.eopkg` and `river-devel-0.5.0-1-1-x86_64.eopkg` plus the `pspec_x86_64.xml` and `abi_*` metadata files. Only `package.yml` and `MAINTAINERS.md` are maintained by hand.