# Scanning-Local-Network-for-Open-Ports
# Objective
The goal is to understand how devices in a local network communicate and to detect which services are running by scanning for open TCP ports. This hands-on task helps build foundational knowledge in network security.

# Tools Used
- Nmap: A powerful network scanning tool
- macOS Terminal: Command-line interface used for executing scans
- IPConfig / ifconfig: For identifying the local IP and interface
  
# Steps Performed
1. Installed Nmap on macOS (M1)
2. Identified the local IP address using:
   ipconfig getifaddr en0
3. Ran a TCP connect scan across the subnet:
   nmap -sT 192.168.0.0/24
4. Saved the scan results:
   nmap -sT -oN scan_result.txt 192.168.0.0/24
5. Documented all open ports and analyzed what services might be running
6. Evaluated potential risks based on common service vulnerabilities

# Files Included
1. scan_result.txt : Raw output from Nmap showing open ports in the local network
2. Task 1_Report : Full analysis and summary of the scan results
3. Terminal.png (Screenshots) : Visual references of terminal outputs
