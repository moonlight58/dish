# dish

A lightweight Linux helper script for installing, updating, launching Vencord, and uninstalling Discord.

## Features

- Installs Discord for Debian-based systems using the official `.deb` package.
- Installs Discord for other Linux distributions using the official `tar.gz` release.
- Updates an existing Discord installation by comparing the installed version with the latest release.
- Downloads and launches the Vencord installer CLI.
- Removes Discord and optionally deletes user configuration.

## Requirements

- `wget`
- `sudo`
- A supported Linux distribution: Debian/Ubuntu-based, Red Hat/Fedora-based, Arch-based, SUSE-based, Gentoo-based, or Slackware-based.

## Installation
To use the script, simply download it and make it executable:

```bash
wget https://raw.githubusercontent.com/moonlight58/dish/main/dish -O dish
chmod +x dish
```

or clone the repository (recommended if you want to create a symbolic link for easier access):

```bash
git clone https://github.com/moonlight58/dish.git
cd dish
chmod +x dish
```

## Usage

```bash
./dish --install
./dish --update
./dish --vencord
./dish --delete
./dish --verbose --install
./dish --verbose --update --vencord
```


> [!NOTE]
> Since it's a personal script and not intended for distribution, it doesn't include error handling or support for all edge cases. Use it at your own risk and feel free to modify it to suit your needs!

If you want to rock it on your daily system, you can create a symbolic link to the script in a directory that's in your `PATH`, such as `/usr/local/bin`:

```bash
sudo ln -s /path/to/dish /usr/local/bin/dish
```

Now you can run `dish` from anywhere in your terminal!

```bash
dish --install
...
```

## Options

- `-h`, `--help`      Show help
- `-i`, `--install`   Install Discord
- `-u`, `--update`    Update Discord
- `-v`, `--vencord`   Launch Vencord CLI
- `-d`, `--delete`    Uninstall Discord
- `-V`, `--verbose`   Enable verbose output

## Notes

- `--install` and `--update` are mutually exclusive.
- The script detects the Linux family from `/etc/os-release` or `/usr/lib/os-release`.

