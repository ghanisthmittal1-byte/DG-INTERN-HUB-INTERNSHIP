# DG Interns Hub --- Week 2

**Intern:** Ghanisth Mittal\
**Period:** Week 2 --- October 2026\
**Focus:** Network traffic analysis, Nmap scanning and Windows security
logging

## Overview

This folder contains Week 2 theory notes, TryHackMe writeups, practical
evidence, PCAP analyses, Windows event investigation material, cheat
sheets, the final report and presentation.

## Environment

-   Kali Linux: `192.168.144.128`
-   Metasploitable 2: `192.168.144.129`
-   Windows: personal Windows 11 laptop
-   Tools: Wireshark, Nmap 7.99, Event Viewer, PowerShell and TryHackMe

All Nmap scanning described here was performed against the user's own
authorised Metasploitable 2 lab VM.

## TryHackMe rooms reported complete

1.  Nmap
2.  Live Host Discovery
3.  Basic Port Scans
4.  Windows Basics
5.  Windows Fundamentals 1
6.  Windows Fundamentals 2

## Practical activities

### Wireshark live capture

-   Captured traffic on Kali `eth0`.
-   Observed TCP handshake and teardown.
-   Inspected DNS, HTTP and ICMP traffic.
-   Used filters such as `tcp`, `dns`, `http`, `icmp` and
    `tcp.flags.syn == 1 && tcp.flags.ack == 0`.
-   Saved a PCAPNG capture and screenshots.

### Nmap scanning

Target: `192.168.144.129` - Host discovery: `-sn` - TCP SYN scan:
`-sS` - Service/version detection: `-sV` - OS detection: `-O` -
Aggressive scan: `-A`

The captured SYN scan showed 18 open TCP ports and 982 closed TCP ports.
Services included FTP, SSH, Telnet, HTTP, MySQL, PostgreSQL, VNC, IRC,
AJP13 and a Tomcat-related service.

### Windows event investigation

-   4624 --- successful logon
-   4625 --- failed logon
-   4720 --- user account created
-   4732 --- member added to a security-enabled local group
-   7045 --- service installed (System log)
-   1102 --- Security audit log cleared; not found in available history

Temporary test accounts were removed after the controlled exercises. The
Security log was not cleared to manufacture Event ID 1102.

### PowerShell

Queried Security Event ID 4625 with `Get-WinEvent`, exported records to
`Failed_Logons_4625.csv` and grouped available records by target
account.

### Sample PCAP analysis

-   `dns.cap` --- DNS PTR and A/AAAA queries and responses.
-   `http.cap` --- HTTP GET request and `200 OK` response.
-   `ipv4frags.pcap` --- IPv4 fragmentation involving ICMP.

## Folder structure

-   `Notes/` --- eight theory notes
-   `Writeups/` --- six TryHackMe writeups and practical writeups
-   `Findings/` --- Windows log exports, Nmap outputs and sample PCAP
    analyses
-   `Captures/` --- screenshots and PCAPNG evidence
-   `Cheat Sheets/` --- Wireshark filters and Windows Event IDs
-   `PDF Report/` --- final report
-   `Presentation Report/` --- final presentation

## Evidence and limitations

This README reflects work reported as completed. Event ID 1102 was not
observed and was not forced by clearing the Security log. Additional
Nmap text-output files and a separate Nmap PCAP file were not visible in
the folder screenshots reviewed when the final report was prepared; add
them if available and required by the submission instructions.

## Learning outcomes

-   Packet analysis and protocol identification with Wireshark
-   Host discovery, port scanning and service identification with Nmap
-   Windows Security event investigation
-   PowerShell event retrieval and CSV export
-   Technical documentation and evidence organisation
