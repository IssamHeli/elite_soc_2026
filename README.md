# elite_soc_2026
This script is designed for Ubuntu 24.04 LTS. It installs the "Golden Stack": Wazuh (SIEM), Shuffle (SOAR), and MISP (Threat Intel), while configuring the kernel for high-performance security indexing.


Run the script:

Bash
chmod +x elite_soc_2026.sh
sudo ./elite_soc_2026.sh
🎓 Why this script is "Elite" for your PFE

Kernel Tuning: Most students fail because vm.max_map_count defaults to 65530, causing Wazuh's database to crash instantly. This script pre-emptively fixes that.

Threat Intel (MISP): Adding MISP moves you from a "Log Collector" to a "Threat Hunter." You can now cross-reference IP addresses found in Wazuh with global malware databases.

Shuffle SOAR: The script includes the permission fix (chown 1000:1000) for the Shuffle database, which is a common "bug" that stops automation workflows from starting.

💡 The "Killer" Presentation Point

During your defense, mention that you used a modular microservices approach:

Host-based Protection: Wazuh Manager.

Automated Response: Shuffle (SOAR).

Intel Correlation: MISP.

Containerization: Using Docker-Compose ensures that your SOC can be scaled or migrated to a real production cloud server in minutes.
