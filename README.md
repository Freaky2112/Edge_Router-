# ![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg) ![Contributions](https://img.shields.io/badge/contributions-welcome-orange.svg) 
![GitHub license](https://img.shields.io/github/license/Freaky2112/Scripts?style=flat-square&color=blue) ![Stars](https://img.shields.io/github/stars/Freaky2112/Scripts) 

# Edge Router Auto Config

An Excel-based configuration generator for Ubiquiti EdgeRouter devices that automatically creates command-line interface (CLI) commands for router setup.

## Overview

This tool simplifies the process of configuring EdgeRouter devices by providing a user-friendly Excel interface. Simply fill in the configuration parameters on the first pages, and the tool will generate all the necessary CLI commands to set up your router.

## Features

- **Automated Command Generation**: Converts user inputs into ready-to-use EdgeRouter CLI commands
- **Excel-Based Interface**: No programming knowledge required - just fill in the fields
- **Time-Saving**: Eliminates manual command writing and reduces configuration errors
- **Comprehensive Setup**: Generates complete command sets for router configuration

## Prerequisites

- Microsoft Excel or compatible spreadsheet application (LibreOffice Calc, Google Sheets, etc.)
- Ubiquiti EdgeRouter device
- SSH or console access to your EdgeRouter

## Usage

1. **Download the Excel File**
   - Clone this repository or download the Excel file directly

2. **Fill in Configuration Parameters**
   - Open the Excel file
   - Navigate to the first pages/sheets
   - Enter your desired router configuration settings (interfaces, VLANs, firewall rules, etc.)

3. **Generate Commands**
   - The tool will automatically generate the CLI commands based on your inputs
   - Review the generated commands in the output section

4. **Apply Configuration**
   - Connect to your EdgeRouter via SSH or console
   - Enter configuration mode: `configure`
   - Copy and paste the generated commands
   - Commit changes: `commit`
   - Save configuration: `save`

## Configuration Options

The Excel tool typically supports configuration for:
- Network interfaces
- IP addressing
- DHCP settings
- NAT rules
- Firewall policies
- VLANs
- Routing protocols
- And more...

## Example Workflow

```bash
# 1. SSH into your EdgeRouter
ssh ubnt@192.168.1.1

# 2. Enter configuration mode
configure

# 3. Paste generated commands from Excel
# [Your generated commands here]

# 4. Commit and save
commit
save
exit
```

## Tips

- Always backup your current configuration before applying new commands
- Test configurations in a lab environment when possible
- Review all generated commands before applying them to production devices
- Keep a copy of the Excel file with your configuration for documentation purposes

## Backup Current Configuration

Before applying new configurations, backup your existing setup:

```bash
show configuration commands > backup-config.txt
```

## License

**Unlicense**

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## Disclaimer

Use this tool at your own risk. Always review generated commands before applying them to production networks. The author is not responsible for any network issues or data loss resulting from using this tool.

## Support

For issues or questions, please open an issue in this repository.

---

## Project Status

![GitHub last commit](https://img.shields.io/github/last-commit/Freaky2112/Edge_Router-)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Freaky2112/Edge_Router-?color=purple)
---
**Note**: This tool is community-developed and is not officially supported by Ubiquiti Networks.
