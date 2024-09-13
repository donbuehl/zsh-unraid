# Unraid Oh My Zsh Plugin

This plugin adds convenient aliases and functions for managing your Unraid server directly from the command line.

## Installation

1. Clone this repository into your Oh My Zsh custom plugins directory:

   ```
   git clone https://github.com/donbuehl/zsh-unraid.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/unraid
   ```

2. Add `unraid` to your plugin list in your `.zshrc` file:

   ```zsh
   plugins=(... unraid)
   ```

3. Reload your `.zshrc` or restart your shell:

   ```
   source ~/.zshrc
   ```

## Features

### Array Management
- `array-start`: Start the Unraid array
- `array-stop`: Stop the Unraid array

### Flash Backup
- `flash-backup`: Create a bootable backup of your unRAID configuration

### User Scripts
- `list-scripts`: List all user scripts
- `run-script <script-name>`: Run a specific user script

### Docker Management
- `docker-list`: List running Docker containers
- `docker-start <container>`: Start a Docker container
- `docker-stop <container>`: Stop a Docker container

### VM Management
- `vm-list`: List all VMs
- `vm-start <vm-name>`: Start a VM
- `vm-stop <vm-name>`: Stop a VM

### Quick Directory Navigation

- `cdboot`: Change to /boot
- `cdextras`: Change to /boot/extras
- `cdappdata`: Change to /mnt/user/appdata
- `cddomains`: Change to /mnt/user/domains
- `cdisos`: Change to /mnt/user/isos
- `cdshare`: Change to /mnt/user/share
- `cddisks`: Change to /mnt/disks

### Plugin Directory Navigation

- `cdplugin <plugin_name>`: Change to the plugin's directory (checks config first, then emhttp)
- `cdpluginconf <plugin_name>`: Change directly to the plugin's config directory
- `cdplugincode <plugin_name>`: Change directly to the plugin's code directory

### System Information
- `unraid_info`: Display a summary of Unraid system information

## Notes

- Some features may require additional plugins or configurations on your unRAID system.
- This plugin is designed to work with Unraid 6.x and later versions.
- Always exercise caution when using commands that modify your array or system configuration.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
