# GNOME Calculator [![Build Status](https://gitlab.gnome.org/GNOME/gnome-calculator/badges/master/build.svg)](https://gitlab.gnome.org/GNOME/gnome-calculator/pipelines)

Calculator is an application that solves mathematical equations and is suitable as a default application in a Desktop environment.

[![Download on Flathub](https://flathub.org/api/badge?svg&locale=en)](https://flathub.org/apps/details/org.gnome.Calculator)

## My Customizations

This fork adds right-click to copy on history entries. Right-clicking any row in the calculation history copies the answer to the clipboard, with a toast notification to confirm.

### Building from source (Arch Linux)

```bash
git clone git@github.com:BubbaSantos/GNOME-Calculator.git
cd GNOME-Calculator
git checkout my-customizations
meson setup builddir
meson compile -C builddir
sudo meson install -C builddir
```

The installed binary goes to `/usr/local/bin/gnome-calculator`, which takes priority over the system package in `/usr/bin`.

### Updating with upstream changes

```bash
git fetch origin
git rebase origin/main
meson compile -C builddir && sudo meson install -C builddir
```

## Useful links

- Homepage: <https://apps.gnome.org/Calculator>
- Report issues: <https://gitlab.gnome.org/GNOME/gnome-calculator/issues/>
- Donate: <https://www.gnome.org/donate/>
- Translate: <https://l10n.gnome.org/module/gnome-calculator/>
