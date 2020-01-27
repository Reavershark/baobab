# Baobab

Baobab is the GNOME [Disk Usage Analyzer](https://wiki.gnome.org/Apps/DiskUsageAnalyzer).

Baobab is a simple application which can scan either specific folders
(local or remote) or volumes and give a graphical representation
including each directory size or percentage in the branch. It also
auto-detects any mounted/unmounted device.


## Hacking

The code lives at GNOME [GitLab](https://gitlab.gnome.org/GNOME/baobab).

Report issues to the GNOME [issue tracking system](https://gitlab.gnome.org/GNOME/baobab/issues).

## Fork

This version requires `vmtouch` installed (https://hoytech.com/vmtouch/).

Instead of showing disk usage, it shows files that are currently mapped in RAM for faster access.
The kernel touches files or parts of files automatically, but with `vmtouch -t path` you can manually touch files.

My use for this was preloading entire games (eg. `vmtouch -tf Games/Osu`).
