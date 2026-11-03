# le-bash

`le-bash` is a prompt-driven command inspector for binary metadata, TLDR,
cheat.sh, manual pages, and executable `--help` output.

Start it with the command you want to inspect:

```bash
./le-bash grep
```

The menu can show binary details, open local references, fetch cheat sheets,
or switch to another command.

## Requirements

Bash, `curl`, and `less` are required. `tldr`, `man`, `col`, `file`, and
`whereis` enable optional reference and metadata features.
Online cheat sheets require an internet connection.

## Run from source

```bash
chmod +x le-bash
./le-bash grep
```

## Debian package

Build the standalone `le-bash` package on Debian or Ubuntu after
installing `debhelper` and `dpkg-dev`:

```bash
dpkg-buildpackage -us -uc -b
sudo apt install ../le-bash_*.deb
```

The package installs `le-bash` in `/usr/bin`.
