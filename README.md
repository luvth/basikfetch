# BasikFetch

A lightweight, fast system information display tool written in Python, inspired by Neofetch.

## Overview

BasikFetch is a simple yet effective tool that displays key system information in your terminal with a minimal ASCII art logo. It's designed to be lightweight and fast, perfect for including in your `.bashrc` or `.zshrc` to display system information on terminal startup.

## Features

- Shows username and hostname
- Displays OS name and version (using pretty name from /etc/os-release)
- Shows kernel version
- Calculates and displays system uptime
- Counts installed packages (based on contents of /usr/bin)
- Displays current shell
- Shows current desktop environment

## Requirements

- Python 3.6+
- psutil package (`pip install psutil`)

## Installation

1. Clone this repository or download the script:
   ```
   git clone https://github.com/luvth/basikfetch.git
   ```
   
2. Make the script executable:
   ```
   chmod +x basikfetch
   ```

3. (Optional) Create a symbolic link to make it available system-wide:
   ```
   sudo mv basikfetch /bin
   ```

## Usage

Simply run the script:

```
basikfetch
```

### Adding to Shell Startup

Add the following line to your `.bashrc`, `.zshrc`, or equivalent shell configuration file:

```
basikfetch
```

## Customization

Feel free to modify the ASCII art or the information displayed by editing the script:

- Change the ASCII art in the `ascii_art` list
- Add or remove system information in the `get_system_info()` function
- Modify colors by changing the ANSI color codes (e.g., `\033[1;34m` for blue)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
