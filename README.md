# Windows Firewall Configuration Hands-On Lab

## Objective
Configure and test firewall rules to allow or block traffic on Windows.

## Environment
- Windows 10/11
- Administrator privileges
- PowerShell

## Steps Performed
1. Opened **Windows Defender Firewall with Advanced Security** (`wf.msc`).
2. Listed current inbound rules.
3. Created a rule to **block TCP port 23 (Telnet)** → `Block-Telnet-Port-23`.
4. Created a rule to **allow TCP port 22 (SSH)** → `Allow-SSH-Port-22`.
5. Verified rules using `Test-NetConnection` **before and after changes**.
6. Exported firewall rules to CSV: [`FirewallRules_Safe.csv`](FirewallRules_Safe.csv)
7. Captured screenshots of all steps for documentation.

## Test Results
- `Block-Telnet-Port-23` successfully blocked port 23.
- `Allow-SSH-Port-22` allowed SSH connections.
- See screenshots in the [`screenshots/`](screenshots/) folder.
- CSV contains a safe summary of firewall rules.

## Lab Document
- Detailed lab report: [Windows Firewall Lab Hands-On](https://docs.google.com/document/d/11YuoZIjO-fHK5oyf3-ywK8f31OY_b-YxQYR4MG9-spg/view)

## Files Included
| File | Description |
|------|-------------|
| `README.md` | Lab report and instructions |
| `FirewallRules_Safe.csv` | Exported firewall rules summary |
| `Windows_Firewall_Lab_HandsOn.pdf` | Detailed lab documentation |
| `Firewall_Interview_QA.md` | Firewall interview questions and answers |
| `screenshots/` | Step-by-step screenshots of lab |
| `screenshots/New_Inbound_rule_creation.png` | New inbound rule creation |
| `screenshots/Status_verification.png` | Verification of rule status |
| `screenshots/step1.png` | Step 1 screenshot |
| `screenshots/step2.png` | Step 2 screenshot |
| `screenshots/step3.png` | Step 3 screenshot |
| `screenshots/step4.png` | Step 4 screenshot |
| `screenshots/step5.png` | Step 5 screenshot |
| `screenshots/Inbound_rules_list.png` | Inbound rules list |
| `screenshots/test_before.png` | Test-NetConnection before rule |
| `screenshots/test_after.png` | Test-NetConnection after rule |

## Learning Outcomes
- Basic firewall management on Windows
- Understanding inbound and outbound rules
- Testing ports with PowerShell
- Exporting firewall rules safely

## Notes
- All files are safe for public sharing; no sensitive data included.
