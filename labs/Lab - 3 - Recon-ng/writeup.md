# Lab 3 - Recon-ng

## Objective:
Learn how to find WHOIS information on a target domain-name.

## Purpose
WHOIS information can consist of location, registation, and experation dates, contact information (email, phone numbers, etc.) and more abouut doamin-name. The purpose of this lab is to usue recon-ng to automate the discovery of this information.

## Tools
- Kali
- Recon-ng

## Walkthrough
- **Step 1:**
  Open the terminal as root and type in `recon-ng`
- **Step 2:**
Recon-ng offers the opportunity for users to create different workstations based on their project needs. We can make one for gathering WHOIS information.
Lets create a new one using `workspaces create whois_recon`.
- **Step 3:**
  We can not start gathering WHOIS information about a target domain-name. Since WHOIS inforamtion is aviable to anyone, it is okay to do this for any doamin.
  The domain we will target is "facebook.com", but you can do this for any other domain. We will need to install modules from the marketplace to search for WHOIS information.
  - We can start by searching WHOIS for all related information regarding a target site. Lets install the WHOIS module.
  `marketplace search whois`. We want to install the _pocs > `marketplace install recon/domains-contacts/whois_pocs`
  - Now we need to load the module `modules load recon/domains-contacts/whois_pocs`
  - To start searching, we need to first set the source `options set SOURCE facebook.com`
  - We can verify our source by running `info`
  - Now simply type `run` to start the search
  - 
