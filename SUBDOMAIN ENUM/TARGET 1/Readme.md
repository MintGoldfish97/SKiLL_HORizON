Subdomain Enumeration

This task is part of my Skill Horizon project, where I document my daily cybersecurity tasks. The goal is to enumerate and list all possible subdomains of the target domain *[yahoo.com]* using three tools and filter which are live.

Target: [yahoo.com]  
Date: [07-09-2025]  
Tools Used:
- *Amass* → for discovering subdomains using passive/active techniques
- *Subfinder* → for collecting real subdomains from multiple sources
- *Assetfinder* → for finding additional subdomains

***

### 1. Amass

*Purpose:*  
Discovers subdomains using both passive and active enumeration.

*Command Used:*
amass enum -d yahoo.com -o yahoo_amass.txt


*Output File:*  
yahoo_amass.txt

### 2. Subfinder

*Purpose:*  
Finds real, publicly available subdomains of the target.

*Command Used:*
subfinder -d yahoo.com -o yahoosubs.txt


*Output File:*  
yahoo_subs.txt

### 3. Assetfinder

*Purpose:*  
Finds additional subdomains.

*Command Used:*
bash
assetfinder --subs-only yahoo.com > yahoo_asset.txt


*Output File:*  
yahoo_asset.txt
[2] Screenshot_20250907-185045_GitHub.jpeg https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/images/82879627/6a00398d-32c4-47e0-aed4-3eb3b8dc1147/Screenshot_20250907-185045_GitHub.jpeg
