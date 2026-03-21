# bloom-packages

PKGBUILDs and pacman repository for Bloom Linux packages.

Packages are automatically built via GitHub Actions and served at:

```
https://bloom-linux.github.io/bloom-packages/
```

## Using the Bloom pacman repo

Add to `/etc/pacman.conf`:

```ini
[bloom]
SigLevel = Never
Server = https://bloom-linux.github.io/bloom-packages/
```

Then:

```bash
pacman -Sy
pacman -S bloom-desktop
```

## Packages

| Package | Description |
|---|---|
| `bloom-desktop` | Meta-package — installs everything |
| `bloom-settings` | Settings panel + volume, brightness, network, power, calendar popups |
| `bloom-shell` | Dynamic island, EWW topbar, theme generation tools |
| `bloom-installer` | Graphical installer, welcome app, first-run wizard |
