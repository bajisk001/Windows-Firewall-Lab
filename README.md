# Firewall Configuration HandsOn Lab - Windows

## Objective
- Configure and test firewall rules to allow/block traffic on Windows.

## Environment
- Windows 10/11
- Admin privileges
- PowerShell

## Steps performed
1. Opened Windows Defender Firewall with Advanced Security (wf.msc).
2. Listed current inbound rules.
3. Created rule to **block TCP port 23 (Telnet)** → named `Block-Telnet-Port-23`.
4. Created rule to **allow TCP port 22 (SSH)** → named `Allow-SSH-Port-22`.
5. Verified rules using `Test-NetConnection` before and after changes.
6. Exported firewall rules to CSV (`FirewallRules_Safe.csv`).
7. Captured screenshots of all steps for documentation.

## Test Results
- `Block-Telnet-Port-23` successfully blocked port 23.
- `Allow-SSH-Port-22` allowed SSH connections.
- See screenshots in `screenshots/` folder or attached `Windows_Firewall_Lab_HandsOn.pdf` file.
- CSV contains safe summary of firewall rules.

## Notes
- No sensitive data included in CSV or screenshots.
