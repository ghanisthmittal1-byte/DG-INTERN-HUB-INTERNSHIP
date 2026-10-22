# DG Interns Hub — Week 1 Cybersecurity Internship

## Overview

This repository documents my Week 1 cybersecurity internship work, including cybersecurity fundamentals, Linux command-line practice, virtual machine lab setup, networking concepts, and hands-on learning through TryHackMe and OverTheWire Bandit.

The main objective was to develop a foundation in cybersecurity, understand basic networking and Linux administration, and document practical exercises in an organized and reproducible manner.

## Objectives

- Understand cybersecurity fundamentals and the CIA Triad.
- Learn the differences between SOC, VAPT, and incident response roles.
- Study the OSI and TCP/IP networking models.
- Practice Linux commands, users, groups, file permissions, and scheduled tasks.
- Understand virtual machine networking and lab isolation.
- Create a basic network map and perform connectivity tests.
- Complete beginner-level TryHackMe rooms.
- Practice Linux command-line challenges through OverTheWire Bandit Levels 0–10.
- Maintain organized notes, screenshots, and technical documentation.

## Lab Environment

| Component | Details |
|---|---|
| Virtualization platform | VMware Workstation |
| Attacker / practice system | Kali Linux |
| Vulnerable practice target | Metasploitable 2 |
| Operating system tools | Linux command line |
| Networking tools | `ip`, `ping`, `nslookup`, `traceroute`, `ss` |
| Documentation | Markdown, Word documents, screenshots, diagrams |
| Learning platforms | TryHackMe and OverTheWire Bandit |

**Safety note:** Metasploitable 2 is intentionally vulnerable. It should be used only in an authorized, isolated lab environment and must not be exposed to public networks.

## Repository Structure

```text
DG Interns Hub/
└── Week 1/
    ├── Notes/
    │   ├── 01_Cybersecurity_and_CIA_Triad.docx
    │   ├── 02_SOC_vs_VAPT_vs_Incident_Responder.docx
    │   ├── 03_OSI_vs_TCPIP_Models.docx
    │   ├── 04_IP_MAC_DNS_DHCP_and_Ports.docx
    │   ├── 05_Linux_File_System_and_Permissions.docx
    │   ├── 06_Threat_Vulnerability_Risk_and_Exploit.docx
    │   ├── 07_VM_Networking_Modes.docx
    │   └── 08_Legal_and_Ethical_Basics_India.docx
    ├── Writeups/
    ├── Findings/
    │   ├── Lab Setup/
    │   ├── Linux Practice/
    │   ├── Network Map - Diagram/
    │   ├── Over the Wire Bandit/
    │   └── TryHackMe/
    │       ├── 01_Search_Skills/
    │       ├── 02_Learning_Cyber_Security/
    │       ├── 03_Linux_Fundamentals_Part_1/
    │       ├── 04_What_is_Networking/
    │       ├── 05_Introductory_Networking/
    │       ├── 06_Networking_Concepts/
    │       ├── 07_Pyramid_of_Pain/
    │       └── 08_Intro_to_LAN/
    ├── Cheat Sheet/
    │   └── Linux_Commands_Cheat_Sheet.docx
    ├── PDF Report/
    ├── Presentation Report/
    └── README.md
```

*Adjust the structure above if your actual folder names or filenames differ.*

## Tasks and Practical Work

### 1. Cybersecurity Fundamentals

Prepared study notes covering:

- Cybersecurity principles and the CIA Triad: Confidentiality, Integrity, and Availability.
- SOC, Vulnerability Assessment and Penetration Testing (VAPT), and incident response.
- OSI and TCP/IP models.
- IP addresses, MAC addresses, DNS, DHCP, and common network ports.
- Linux file systems and permissions.
- Threats, vulnerabilities, risks, and exploits.
- Virtual machine networking modes.
- Legal and ethical considerations in cybersecurity.

### 2. Linux Command-Line Practice

Used Kali Linux to practice basic Linux administration and system inspection.

Commands covered include:

```bash
whoami
hostname
cat /etc/os-release
pwd
ls -la
ip a
ip route
find
grep
ps aux
sudo ss -tulpn
chmod
chown
groups
getent group
crontab -e
```

Practical exercises included:

- Inspecting the operating system and network configuration.
- Creating users and groups.
- Configuring shared directory permissions.
- Testing authorized group-based file access.
- Searching files and inspecting running processes.
- Configuring a cron job and checking its output.

### 3. Networking and Network Mapping

Practiced basic network discovery and connectivity checks using:

```bash
ip a
ip route
cat /etc/resolv.conf
ping -c 4 8.8.8.8
ping -c 4 google.com
nslookup google.com
traceroute google.com
```

The network mapping exercise documented the Kali Linux virtual machine, its network interface, gateway, DNS configuration, and internet connectivity path.

**Evidence:** Refer to `Findings/Network Map - Diagram/` for the network diagram and supporting screenshots, where available.

### 4. Virtual Machine Lab Setup

The lab environment includes Kali Linux and Metasploitable 2 running in VMware Workstation.

The setup work focused on:

- Identifying available virtual machines.
- Inspecting network interfaces and IP configuration.
- Understanding NAT, bridged, and host-only networking.
- Keeping vulnerable targets isolated from untrusted networks.
- Documenting lab configuration and test results.

**Evidence:** Refer to `Findings/Lab Setup/`. Record only configurations and connectivity tests that have actually been verified.

### 5. OverTheWire Bandit

Practiced OverTheWire Bandit Levels 0–10 to strengthen Linux command-line and file-handling skills.

| Level | Main concept |
|---|---|
| 0 | Connecting through SSH and reading a file |
| 1 | Accessing a filename containing a special character |
| 2 | Handling filenames containing spaces |
| 3 | Finding hidden files |
| 4 | Identifying file types |
| 5 | Searching for files by properties |
| 6 | Searching by owner, group, and size |
| 7 | Searching file contents with `grep` |
| 8 | Using `sort` and `uniq` |
| 9 | Extracting readable strings |
| 10 | Decoding Base64 data |

**Evidence:** Refer to `Findings/Over the Wire Bandit/` for the write-up and screenshots.

Passwords, tokens, and other credentials should never be included in this repository or in public screenshots.

### 6. TryHackMe Rooms

The following beginner rooms were completed according to the recorded progress:

| No. | Room | Link |
|---|---|---|
| 1 | Search Skills | [Open room](https://tryhackme.com/room/searchskillscS) |
| 2 | Learning Cyber Security | [Open room](https://tryhackme.com/room/beginnerpathintro) |
| 3 | Linux Fundamentals Part 1 | [Open room](https://tryhackme.com/room/linuxfundamentalspart1) |
| 4 | What Is Networking? | [Open room](https://tryhackme.com/room/whatisnetworking) |
| 5 | Introductory Networking | [Open room](https://tryhackme.com/room/introtonetworking) |
| 6 | Networking Concepts | [Open room](https://tryhackme.com/room/networkingconcepts) |
| 7 | Pyramid of Pain | [Open room](https://tryhackme.com/room/pyramidofpainax) |
| 8 | Intro to LAN | [Open room](https://tryhackme.com/room/introtolan) |

**Evidence:** Refer to the corresponding folders in `Findings/TryHackMe/`. Completion screenshots should be included where available.

## Linux Command Cheat Sheet

A separate Linux command cheat sheet was prepared to provide quick references for commonly used commands, including file management, system information, networking, searching, permissions, processes, and scheduled tasks.

**File:** `Cheat Sheet/Linux_Commands_Cheat_Sheet.docx`

## Key Learning Outcomes

Through these activities, I developed practical familiarity with:

- Linux command-line navigation and basic administration.
- File permissions, ownership, users, and groups.
- Basic network configuration and connectivity troubleshooting.
- Virtual machine networking and safe lab practices.
- Searching files and analyzing system information.
- Fundamental networking concepts and common protocols.
- Beginner-level cybersecurity learning platforms.
- Technical documentation and evidence organization.

## Ethical and Safety Guidelines

- Perform security testing only on systems for which authorization has been granted.
- Keep intentionally vulnerable virtual machines isolated.
- Do not expose credentials, challenge passwords, tokens, or sensitive information.
- Document findings accurately and distinguish verified results from assumptions.
- Follow applicable laws, platform rules, and responsible disclosure practices.

## Final Deliverables

The Week 1 work is organized into the following categories:

- Cybersecurity theory notes.
- Linux command cheat sheet.
- Virtual machine lab evidence.
- Linux practice screenshots.
- Network map and connectivity evidence.
- OverTheWire Bandit write-up.
- TryHackMe room evidence.
- Final PDF report and presentation, once prepared.

## Conclusion

Week 1 provided a foundation in cybersecurity concepts, Linux administration, networking, virtual lab environments, and beginner-level hands-on security exercises. The documentation and evidence folders organize the work completed and provide a reference for future cybersecurity learning.

**Prepared for:** DG Interns Hub — Week 1 Cybersecurity Internship

**Author:** Ghanisth Mittal
