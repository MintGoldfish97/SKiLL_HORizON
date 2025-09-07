
Subdomain Enumeration

This task is part of my Skill Horizon project, where I document my daily cybersecurity tasks. The goal is to enumerate and list all possible subdomains of the target domain [bugcrowd.com] using three tools and filter which are live.

Target: [bugcrowd.com]
Date: [07-09-2025]
Tools Used:

Amass → for discovering subdomains using passive/active techniques
Subfinder → for collecting real subdomains from multiple sources
Assetfinder → for finding additional subdomains
1. Amass
Purpose:
Discovers subdomains using both passive and active enumeration.

Command Used: amass enum -d bugcrowd.com -o bugcrowd_amass.txt

Output File:
bugcrowd_amass.txt

2. Subfinder
Purpose:
Finds real, publicly available subdomains of the target.

Command Used: subfinder -d bugcrowd.com -o bugcrowd_subs.txt

Output File:
bugcrowd_subs.txt

3. Assetfinder
Purpose:
Finds additional subdomains.

Command Used: assetfinder --subs-only bugcrowd.com > bugcrowd_asset.txt

Output File:
bugcrowd_asset.txt
