 ____  __.____ _______    __________      _________ __________    _____   
|    |/ _/_   |\      \  /  _____/  \    /  \   _  \\______   \  /     \  
|      <  |   |/   |   \/   \  __\   \/\/   /  /_\  \|       _/ /  \ /  \ 
|    |  \ |   /    |    \    \_\  \        /\  \_/   \    |   \/    Y    \
|____|__ \|___\____|__  /\______  /\__/\  /  \_____  /____|_  /\____|__  /
        \/            \/        \/      \/         \/       \/         \/ 
# wifihacker_script
This repository contains a Bash script to install Realtek Wi-Fi drivers, Wifite dependencies, and other tools for wireless network analysis. The script is designed to run on Kali Linux, but it may also work on other Debian-based distributions.

## Prerequisites
- A Linux-based system, ideally Kali Linux or another Debian-based distribution.
- Root access or appropriate permissions to run system-level commands.
- An internet connection to download packages and clone Git repositories.

## How to Use the Script
1. **Clone the Repository**:
   - Clone the GitHub repository containing the script to your local machine:
     ```bash
     git clone https://github.com/Sudocod3r/wifihacker_script.git
     ```
   - Navigate to the cloned repository directory:
     ```bash
     cd /wifihacker_script
     ```

3. **Make the Script Executable**:
   - Change the script's permissions to make it executable:
     ```bash
     chmod +x install_wifi_drivers.sh
     ```

4. **Run the Script**:
   - To execute the script, run:
     ```bash
     ./install_wifi_drivers.sh
     ```
   - If you need root permissions, use `sudo` to run it with elevated privileges:
     ```bash
     sudo ./install_wifi_drivers.sh
     ```
   - Follow the instructions provided in the script. It will update the system, reboot if needed, and then proceed to install various dependencies and tools.

## What the Script Does
- **Updates the System**: Ensures that all packages are current, which helps avoid compatibility issues.
- **Installs Wi-Fi Drivers**: Installs Realtek Wi-Fi drivers and related tools like `dkms` and `build-essential`.
- **Clones and Compiles Software**: Clones repositories and compiles tools like `rtl8812au`.
- **Installs Wireless Network Tools**: Installs `hcxdumptool`, `hcxpcaptool`, and `Pyrit`.
- **Installs Database Support**: Installs PostgreSQL for database support.
- **Installs Python Packages**: Installs Python packages `psycopg2` and `scapy`.
- **Final System Update and Reboot**: Ensures system stability by updating everything after installations.

## Troubleshooting
- **Errors During Installation**:
  - Check for any error messages in the script output and resolve them accordingly.
  - If the script fails to update, ensure you have a stable internet connection.
  - If the script fails due to permissions, ensure you're running it with `sudo`.
- **Tool Installation Failures**:
  - If `pyrit` or `scapy` fail to install, check if they are installed by running `command -v pyrit` and `command -v scapy`.
  - If `hcxdumptool` or `hcxpcaptool` installation fails, ensure their Git repositories are accessible.
- **Rebooting**:
  - If the system reboots, you must re-run the script to complete all steps.
  - If the script doesn't continue after a reboot, remove lines 1-11 from kali_wifite_dependancies_ALFA_Drivers, and ensure you're in the correct directory and try running it again.
  - Run one command at a time or update, upgrade, and reboot if script fails
## Contributing
If you encounter issues or have suggestions for improving the script, feel free to open an issue or submit a pull request in this repository :) 


