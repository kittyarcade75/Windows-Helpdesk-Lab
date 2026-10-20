# Objective
Practice basic Windows network troubleshooting commands and document the results

# Lab Environment 
Operating System: Windows 11

Tools: Windows PowerShell

Lab Type: local troubleshooting exercise 

# Trouble Shooting Commands
COMMAND 1: VIEW IP CONFIGURATION

I entered the command "ipconfig /all" into PowerShell to display network adapters, IP addresses, DNS servers, and other network configuration details. 

--------------------------------

COMMAND 2: TEST CONNECTIVITY

I entered the command "ping 1.1.1.1" into PowerShell to test whether the computer can reach a public IP address using ICMP and if the network/destination allow it. 

------------------------------------

COMMAND 3: TEST DNS RESULTS

I entered the command "nslookup github.com" into PowerShell to display IP configuration details for network interfaces. 

---------------------------------------------------------

COMMAND 4: VIEW NETWORK CONFIGURATION WITH POWERSHELL

I entered the command "Get-NetIPConfiguration" into PowerShell to display IP configuration details for network interfaces. 


# Results 
COMMAND 1: The Wi-Fi adapter has IPv4, default gateway, DNS server, and DHCP configuration fields. Further connectivity and DNS tests are needed to determine whether network access is functioning correctly. 

COMMAND 2: I received replies with a 0% packet loss and response times within the 50-150 ms range. This indicates a successful IP connectivity to the destination during the test.

COMMAND 3: Successfully resolved the domain and returned with one IP address. 

COMMAND 4: Command ran successfully. Output included InterfaceAlias, IPv4Address, IPv4DefaultGateway, and DNSServer. 


# Troubleshooting Analysis 
No issues were discovered. 

# Notes
No notes.
