+++
title = 'SubMon'
description = 'Subdomain monitor for bug bounty hunters: scheduled scans that send a Discord alert the moment a target gets a new subdomain.'
weight = 4
stack = ['Python', 'FastAPI', 'SQLModel', 'React', 'Docker']
repo = 'https://github.com/liuyc26/SubMon'
+++
<!-- DRAFT from the README. Please check and add why you built it / any results. -->

**Problem.** In bug bounty, being *first* to a new asset matters as much as finding the bug.

**What I built.** A dashboard where you add targets, run or schedule scans (subfinder, dnsx, httpx), and see which subdomains are new or missing since the last scan, with page titles. A background worker sends a Discord notification whenever new subdomains appear.

**Result.** _[Add: what it found, how long you've run it, or what you learned]_
