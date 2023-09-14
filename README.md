# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## OUTPUT:
![1](https://github.com/Aakash0407/Enumeration/assets/118799103/a588360a-5d51-4d26-8322-2f6ebe032e87)
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## OUTPUT:
![2](https://github.com/Aakash0407/Enumeration/assets/118799103/f3e518cd-6e9e-4a68-8d7c-8814a8755cfb)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT:
![3](https://github.com/Aakash0407/Enumeration/assets/118799103/dc9f230f-dda7-4b8f-a781-9fd26086ec1f)
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT:
![4](https://github.com/Aakash0407/Enumeration/assets/118799103/97ced70a-7a07-4633-a8c1-d2f6b675c4a6)
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT:
![5](https://github.com/Aakash0407/Enumeration/assets/118799103/277b9853-d670-482f-919a-7e3742e044ca)
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT:
![6](https://github.com/Aakash0407/Enumeration/assets/118799103/2ca05ba5-465e-4d79-bf68-8bd726ea6482)
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
![7](https://github.com/Aakash0407/Enumeration/assets/118799103/1e930c95-fe58-473b-a483-71d5d7527307)
#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![8](https://github.com/Aakash0407/Enumeration/assets/118799103/bff6b1fa-db5a-4634-9e87-09d9ebd0da4f)
![9](https://github.com/Aakash0407/Enumeration/assets/118799103/340db1a8-7257-4426-9b9e-6cdb8d653240)

##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:
![10](https://github.com/Aakash0407/Enumeration/assets/118799103/68bd4daa-782d-43ff-bf7d-ab03a8a0ab7b)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![11](https://github.com/Aakash0407/Enumeration/assets/118799103/d8162783-ec5d-4ad9-b1c9-14e3e26dce67)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
![12](https://github.com/Aakash0407/Enumeration/assets/118799103/b7b2b3d4-681d-457e-987f-fa9982d42525)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
![13](https://github.com/Aakash0407/Enumeration/assets/118799103/ff539a92-be6e-40a3-8c46-d9b223a62e21)
## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![14](https://github.com/Aakash0407/Enumeration/assets/118799103/16652a98-4067-4b41-ae7f-2606f57b747a)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

