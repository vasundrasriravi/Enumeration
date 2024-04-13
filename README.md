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

## Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![Screenshot 2024-04-13 131900](https://github.com/vasundrasriravi/Enumeration/assets/119393983/8cf39b67-61fa-4a37-be6f-80ef3b54aa11)


## filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![Screenshot 2024-04-13 132358](https://github.com/vasundrasriravi/Enumeration/assets/119393983/28fa1d08-331b-4bfd-81cf-f8e4454be668)

## intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![Screenshot 2024-04-13 132544](https://github.com/vasundrasriravi/Enumeration/assets/119393983/1209fcc1-1016-4170-9664-4c32301077c7)


## inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot 2024-04-13 132634](https://github.com/vasundrasriravi/Enumeration/assets/119393983/45ee1ba6-b2a1-4c12-b368-4766dfba96d6)



## intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot 2024-04-13 132744](https://github.com/vasundrasriravi/Enumeration/assets/119393983/6e8f3c9c-dc4f-422b-8a45-77ea3655c0fe)



## link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![Screenshot 2024-04-13 132844](https://github.com/vasundrasriravi/Enumeration/assets/119393983/240b5ced-bba7-41be-b689-93438fd43000)


## cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2024-04-13 141738](https://github.com/vasundrasriravi/Enumeration/assets/119393983/ad5e601a-ecce-46e1-ae2a-ab380a47b7a1)

## DNS Recon
![Screenshot 2024-04-13 134717](https://github.com/vasundrasriravi/Enumeration/assets/119393983/37bc0649-37fa-40c6-a6af-2e8f81aea2af)
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion.

## dnsenum
![Screenshot 2024-04-13 135628](https://github.com/vasundrasriravi/Enumeration/assets/119393983/9c954580-ec7e-4d25-932c-3c8a5581de43)
![Screenshot 2024-04-13 140236](https://github.com/vasundrasriravi/Enumeration/assets/119393983/624f1cc9-ba2d-4a25-a468-09c054168b5d)
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


## smtp-user-enum
![Screenshot 2024-04-13 140256](https://github.com/vasundrasriravi/Enumeration/assets/119393983/da303347-4e84-435d-b282-284017f04b00)
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same

# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

## nmap –script smtp-enum-users.nse <hostname>
![Screenshot 2024-04-13 140316](https://github.com/vasundrasriravi/Enumeration/assets/119393983/5b9a6f7f-17b7-4030-8473-b6ab4c2c3a67)
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
