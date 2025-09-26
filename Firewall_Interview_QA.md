# Firewall Interview Q/A

## 1. What is a firewall?

A firewall is a security system that monitors and controls network traffic between your computer or network and the outside world. It decides what traffic is allowed in or out based on predefined rules.

**Key points:**
- Acts as a barrier between trusted and untrusted networks.
- Can be hardware-based (like a router firewall) or software-based (like Windows Firewall or UFW).
- Protects against unauthorized access, malware, and network attacks.

**Layman analogy:**  
Like a security guard at a building entrance checking who can come in or go out.

---

## 2. Difference between stateful and stateless firewall


| Feature | Stateful Firewall | Stateless Firewall |
|---------|-----------------|-----------------|
| Tracks connections | Yes, keeps track of ongoing connections | No, checks packets individually |
| Security level | Higher, can detect unexpected packets | Lower, only applies simple rules |
| Example | Windows Firewall, Cisco ASA | Basic packet filters, older routers |
| Best for | Complex networks with dynamic traffic | Simple networks or basic filtering |

**Layman explanation:**  
- **Stateful** = remembers past traffic, smarter decisions.  
- **Stateless** = no memory, only checks each packet separately.

---

## 3. What are inbound and outbound rules?
 
- **Inbound rules:** Control traffic coming into your system/network.  
  *Example:* Allow SSH on port 22, block Telnet on port 23.  
- **Outbound rules:** Control traffic going out from your system/network.  
  *Example:* Block access to suspicious websites.

**Layman analogy:**  
- Inbound = “Who can enter my house?”  
- Outbound = “Where can my house send information?”

---

## 4. How does UFW simplify firewall management?
 
UFW (Uncomplicated Firewall) is a Linux command-line tool that makes managing firewall rules easy.

**Key points:**  
- Provides simple commands like `ufw allow 22` or `ufw deny 23`.  
- Handles complex iptables rules automatically behind the scenes.  
- Good for beginners or small servers who don’t want to write raw iptables commands.

**Layman analogy:**  
Like a simple remote control for a complex security system.

---

## 5. Why block port 23 (Telnet)?
 
- Telnet (port 23) is an old protocol for remote access.  
- Security risk: Transmits data in plain text, including passwords.  
- Blocking it prevents attackers from intercepting sensitive info.  
- Modern alternatives: SSH (port 22) which encrypts traffic.

---

## 6. What are common firewall mistakes?

- Leaving default rules open (allowing all traffic).  
- Blocking necessary services accidentally.  
- Not updating firewall rules when network changes.  
- Ignoring logging and monitoring, so attacks go unnoticed.  
- Using a single layer of protection, relying only on firewall.

**Tip for interviews:**  
Always mention “monitoring and updating rules regularly”.

---

## 7. How does a firewall improve network security?

- Filters traffic to prevent unauthorized access.  
- Blocks malicious traffic like viruses, malware, or attacks.  
- Protects sensitive data from leaving the network.  
- Works as first line of defense along with antivirus and intrusion detection systems.

**Layman analogy:**  
Like a checkpoint that only lets safe, authorized traffic in and out.

---

## 8. What is NAT in firewalls?

NAT (Network Address Translation) is a technique where the firewall or router changes the source or destination IP addresses in network packets.

**Key points:**  
- Helps hide internal IP addresses from the outside world.  
- Allows multiple devices to share a single public IP.  
- Can be used in firewalls for security and IP management.

**Layman analogy:**  
Like a translator or middleman that hides your home address when sending letters outside.
