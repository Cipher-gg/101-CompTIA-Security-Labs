# Lab 1 Credential Harvesting Using Site Cloning

## Tools: 
- Kali Linux
- setoolkit

SETOOLKIT - The Social-Engineer Toolkit (SET) is an open-source Python-driven tool aimed at penetration testing around Social-Engineering. Some attack vectors that are including in SET are 
- Spear-Phising
- Web Sites
- Malicuous USB/DVD/CDs
- Arduino
- Wireless Access Points
- QRCodes
- etc.

## Lab Walkthrough
- **Step 1:**
  Boot up the Kali machine and make sure it is up to date. Run <sudo apt update && sudo apt upgrade>
  Next start the **SET: Social Engineering Toolkit** as root. 
  Make sure SET configuration is updated (Press **3**)
- **Step 2:**
  From the menu select option **1** for **Social-Engineering Attacks**, then select the option **2** for **Website Attack Vectos**. This is where you can decided what kind of website attack you want to do. For this lab we are goinig to select option 3, the **Credential Harvester Attack Method**.
- **Step 3:**
  You will be asked how you would like to make this site; from a template, site cloner, or custom import. Select option 2 **Site Cloner**. 
- **Step 4:**
  The Social-Enineer Toolkit (SET) will then ask you for an IP address that it can send the POST requests from the cloned website back to your machine. By default SET will detect your IP address automatically. 
  Once you tell SET you want to clone a website, it will ask you for the URL of the site you want to clone. For this example I will be using Facebook, [https://www.facebok.com/](https://www.facebook.com/)
  
