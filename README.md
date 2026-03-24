# Dish

A simple bash script to manage Discord installation on Linux systems.
Because there's no auto update for discord package 

## Features

- Install Discord (deb or tar.gz based on your Linux distribution)
- Update Discord
- Launch Vencord CLI
- Uninstall Discord
- Verbose mode for detailed output

## Usage

```bash
./dish [options]
```

### Options

- `-h, --help`: Show help message
- `-i, --install`: Install Discord
- `-u, --update`: Update Discord
- `-v, --vencord`: Launch Vencord CLI
- `-d, --delete`: Uninstall Discord
- `--verbose`: Enable verbose output

## Requirements

- wget
- Bash
- Linux system (Debian-based, Red Hat-based, Arch-based, SUSE-based, Gentoo-based, or Slackware-based)

## Installation

Clone the repository and make the script executable:

```bash
git clone https://github.com/moonlight58/dish.git
cd dish
chmod +x dish
```

Then run `./dish --help` for usage information.