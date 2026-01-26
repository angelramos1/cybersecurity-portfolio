# Offensive Security Intro

**Date Completed:** January 26, 2026  
**Difficulty:** Easy  
**Room Link:** https://tryhackme.com/room/introtooffensivesecurity

## Overview
This room introduced me to offensive security by having me find vulnerabilities in a fake banking application. The goal was to discover hidden pages that could be exploited.

## What I Learned
- How to enumerate web directories to find hidden pages
- Using directory brute-forcing tools to discover content
- Understanding that attackers look for pages developers forgot to secure
- The importance of proper access controls on web applications

## Tools Used
**DirBuster (dirb command)**
```bash
dirb http://fakebank.thm
```
This tool searches for hidden directories and files on web servers by trying common names from a wordlist.

## Process
1. Accessed the FakeBank application
2. Opened the terminal on the TryHackMe machine
3. Ran `dirb` against the target URL
4. Analyzed the output - lines starting with `+` indicated discovered pages
5. Found two hidden URLs that weren't linked from the main site

## Key Takeaway
Many web vulnerabilities come from misconfigurations or forgotten pages rather than complex exploits. Simple enumeration tools like dirb can reveal security issues that developers overlooked. This shows why security needs to be considered throughout the entire development process, not just added at the end.

## Reflection
This was my first hands-on experience with offensive security tools. It was interesting to see how easy it is to find hidden content on websites. It makes me think about the applications I'll build as a software engineer - I need to ensure nothing is left exposed unintentionally.
