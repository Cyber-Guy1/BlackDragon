# Black-Dragon V2.0 [VIPX Edition]
An Advanced Automation Tool For Web-Recon Developed For Linux Systems

<div align="center">
	
<img src='VIPX.png' width='70%' height='70%'>

</div>

## What Is Black Dragon ?

It's A Tool To Automate The Web Reconnaissance Proccess, Which Make It Easier To Gather Informations About Your Target. This Tool Will Help You In Your Bug Hunting Or Web Penetration Testing Operation Because It Not Only Gather Informations About The Target, But Also It Arranges All These Information In A Structed Way Which Makes You Analyse The Data In A Good Way.

This Tool Works In Linux Systems, Specially In Debian & Debian Based Systems Like:

1. Kali Linux
2. Parrot OS
3. Ubuntu
4. Debian
5. Back Box

And Other Debian Based Linux Distro's

## What Is The Best Use For This Tool ?

This Is An Automated Tool, So Simply You Give It A Target Then Simply The Tool Took All The Information & And Save The Results In Ordered Directories & Files, But When You Do The Recon You Just Use This Tool, But Also You Should Do Some Manual Activity, This Mindmap Shows The Whole Operation Of BlackDragon Recon Methodology:

<div align="center">
	
<img src='BlackDragon - Recon.png' width='100%' height='100%'>

</div>

So Any Tool Based Recon In This Methodology, I Put It Here In This Automation Tool, But I Prefer To Do So Recon Manually, So First You Should Search Deeply In The IOT Search Engines Like:

- [x] [Shodan.io](https://shodan.io)
- [x] [Censys.io](https://censys.io)
- [x] [Zoomeye](https://zoomeye.org)

Also You Should Search In Some FTP Search Engines Like:

- [x] [SearchFTPs](http://searchftps.net/)
- [x] [Search Archive](http://archie.icm.edu.pl/)
- [x] [File Searching](http://www.filesearching.com/)  
- [x] [Free Ware Web](http://www.freewareweb.com/ftpsearch.shtml)
- [x] [MMNT.ru](https://www.mmnt.ru/int/)
- [x] [FTP Sites](http://www.ftp-sites.org/)

When You Wanna Make A Powerfull Recon, You Should Also Look At:

- [x] [Hunter.io](https://hunter.io/) -> For Target Email Searching 
- [x] [Public-WWW](https://publicwww.com) -> For String Searching In Public Source Codes

## What Did This Tool Do:

- Subdomain-Gathering Using:

- [x] Subfinder
- [x] Sublist3r
- [x] Amass

	- Enum:
		- Active Recon 
		- Passive Recon
		
	- Intel:
		- Active Recon
	
- [x] Assetfinder
- [x] Knockpy
- [x] github-subdomains


- Getting The Whole Subdomain Gathered Then Filter The Unique Domains And Extract The Only Live Subdomain Using:

- [x] httpx


- Fuzzing The Application Target Based Using:

- [x] Gobuster
- [x] Dirsearch
- [x] Dirb


- Endpoints Gathering Using:

- [x] Waybackurls
- [x] github-endpoints


- DNS Information Gathering Using:

- [x] DNSMap
- [x] DNSEnum   
- [x] MassDNS
- [x] Gobuster

- Port Scanning
- [x] rustscan

## What's New In This Version [2.0] ?

- Bug Fixes

- Amass Enum Passive & Active Recon

- Amass Intel Passive & Active Recon

- Domains Ports Discovery & Screen Shootig

- Vulnerability Scanning:

	- CVE Scanning
	- Workflow Scanning
	- Default-Logins Scanning
	- Takeovers Scanning
	- Exposed Panels Scanning

- IoT Search Engine Recon [Shodan]:
	
	- Domain Info Gathering
	- Host Info Gathering
	- Honeypot Checker

- HTTP & HTTPS Filtering

- Smarter Functionalities 

## Installation

### Be Sure To Delete The Previous Version The Install The New

First Delete The Previous Version If Exists:

`rm -rf BlackDragon`

Then Simply After Cloning The Repository By Typing :

`git clone https://github.com/Cyber-Guy1/BlackDragon.git` 

Then Open Up The BlackDragon Directory:

`cd BlackDragon/`

After That Give The Execution Permission To The Installation Script And The Tool Script:

`chmod +x install; chmod +x Black-Dragon`

Finally Run The Installation Script:

`./install`

## Tool Using Syntax:

Simply:

`./Black-Dragon example.com`

> Note: DO NOT Add http:// or https:// In The Domain, The Tool Do This Automatically

## Tool Output Example

<pre>
cyber-guy@Security:~/BlackDragon$ ./Black-Dragon google.com

                                         `.-:/+oosssoo+/::-.
                                    `:oydmNNMMMMMMMMMMMMMNNNmdyo/-`
                                   -dNMMMMMMMMMMMMMMMMMMMMMMMMMMMNmh+-`
                                    ........-:/oydNMMMMMMMMMMMMMMMMMMNms:`
                                           .:os  `.yMMMMMMMMMMMMMMMMMMMMNd+`
                                         :ymMm/ ``.oMMMMMMMMMMMMMMMMMMMMMMMm/
                                   ..++yhNMMMmmmmmmMMMMMMMMMMMMMMMMMMMMMMMMMMh.
                                `/ymNMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMs:omd.
                              .smMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM/  `+y`
                             /NdoyMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMN/   .-
                            `NMddNMMMMMMNmNMddddmNNMMMMMMMMMMMMMMMMMMMMMMMMMy-
                            `oddddhyso/-.`.-` ```.-:ohNMMMMMMMMMMMMMMMMMMMMMMNy-
                              ```     ``..            .+dMMMMMMMMMMMMMMMMMMMMMMNo
                                  ./ohdmmo```..         `/mMMMMMMMMMMMMMMMMMMMMMMs
                               .+hNMMMMMMNmmmmm:.....`    .dMMMMMMMMMMMMMMMMMMMMMM-
                             `omMMNNmmmNNMMMMMMMNmmm+-.    `mMMMMMMMMMMMMMMMMN+:yM/
                            `hMmy/-.....-:/ohmNMMMMo        +MMMMMMMMMMMMMMMMh  `m`
                            sMd.             `-sNMMs        -MMMMMMMMMMMMMMMMs  ..
                            NM+                 .yMN        +MMMMMMMMMMMMMMMM/
                            NMh`                 `hm       .mMMMMMMMMMMMMMMMm`
                            sMMy.                 --      :mMMMMMMMMMMMMMMMM/
                            `dMMNs-`                   `:yMMMMMMMMMMdymMMMN+
                             .hMMMMds/-.`         `.-+ymMMMMMMMMMMNo` hMMm:
                               +mMMMMMMNdhyysssyyhdNMMMMMMMMMMMMms.  +Mmo`
                                `/ymMMMMMMMMMMMMMMMMMMMMMMMMNmh/`   +s:`
                                   `:ohmNNMMMMMMMMMMMMNNNdy+:`
                                        .-:/+osssso++/:.`

			          An Automated Tool For Web-Recon
					Developed By Momen Ali
					    The CyberGuy
						v-2.0

                                         _    __________ _  __
                                        | |  / /  _/ __ | |/ /
                                        | | / // // /_/ |   / 
                                        | |/ _/ // ____/   |  
                                        |___/___/_/   /_/|_|  
                      


====================================
               Banner                  
====================================

[+] Target Domain => google.com
[+] Date => 05-05-2021
[+] Current User => cyber-guy

-------------------------------------

[+] Current Recon Path: => /home/cyber-guy/BlackDragon/google.com/05-05-2021

====================================

</pre>

Stay Secure ;)


<hr>


## [GPL V3 License](https://github.com/Cyber-Guy1/BlackDragon/blob/main/LICENSE.md) 
<img src="gplv3-with-text-136x68.png">
