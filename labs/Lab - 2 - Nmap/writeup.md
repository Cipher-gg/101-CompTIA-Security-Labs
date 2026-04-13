# Lab 2 - Nmap

## Objectives:
Learn how to scan a host using Nmap and understand the results

## Purpose:
Nmap (Network Mapper) is one of the most common tools used among hackers and system administrators. It is used to scan a host, which can be a server, pc, network, etc. When running an Nmap scan, the goal is usually to discover various pieces of information about a target system or network. Examples of such information include: the deives that are connected to a network, the ports that are open on a device, the servies that are running on these ports, whether the devies is up, and whether there is a firewall protecting the, etc. 

## Tools:
- Kali Linux
- Nmap (Network Mapper)

## Walkthrough:
- **Task 1:**
  Nmap comes pre-installed on Kali. Just open the terminal and type, `nmap scanme.nmap.org` This will initiate a scan of the target and will attempt to determine which ports are open and what servies are open on these ports. This was a very basic scan and it will only scan the top 1000 ports for basic information.
- **Task 2:**
  We are going to scan the same target `scanme.nmap.org` but with a more advanced scan. Let's say we want to determine the versions for the servies that are running on each port, so that we can determine if they are out of date and potentially vulnerable to exploitation. We also want to determine the operating system of the webserver running the target site. This sacn will require the use of root for the scan. `sudo nmap -v -sT -sV -O scanme.nmap.org`
  - v > increase verbosity level
  - sT > TCP SYN/Conect()/ACK/Window/Maimon scans
  - sV > Probe open ports to determine service/version info
  - O > Enable OS detection
  - A > will scan a target using the -sS, -sV, and -O flags
