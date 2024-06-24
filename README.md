# Nmap-Automation-Script

Streamline network reconnaissance with this advanced Nmap automation script. Perform default, service, and all-port scans, including options for fast mode and verbosity. Automates detection and scanning of newly discovered open ports, utilizing specified start and end port ranges for comprehensive security audits and vulnerability assessments.

## Installation

### Clone the Repository
Clone the repository using Git:

```bash
git clone https://github.com/NitheshD05/Nmap-Automation-Script.git
cd Nmap-Automation-Script
```

### Install Required Modules and Tools
Ensure you have Python 3.x installed. Use pip to install the required modules:

````bash
pip install -r requirements.txt
````

### Usage
 Run the script with Python 3.x, providing the target IP address or hostname:

````bash
python3 nmap.py 10.10.10.10
````
This command initiates an intense scan sequence, including Default Scan, Service and Script Scan, and All Port Scan. It then performs a Script and Service scan specifically for newly identified ports from the All Port Scan.  

### Options and Examples
The script supports various options to customize scans:

````bash
python3 nmap.py --help                
usage: nmap.py [-h] [-d] [-s] [-a] [--speed] [--start START] [--end END] [-v] target

🔓 Unleash the Nmap Fury! 🔓

positional arguments:
  target           Target IP address or hostname

options:
  -h, --help       show this help message and exit
  -d, --default    Run only the default scan (default: False)
  -s, --service    Run only service and script scan (default: False)
  -a, --all-ports  Run only all-port scan (default: False)
  --speed          Run scans in fast mode (default: False)
  --start START    Start port for scanning (default: None)
  --end END        End port for scanning (default: None)
  -v, --verbose    Run scans in verbosity mode (default: False)
````

