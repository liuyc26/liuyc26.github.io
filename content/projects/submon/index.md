+++
title = 'SubMon'
description = 'Subdomain monitor for bug bounty hunters: scheduled scans that send a Discord alert the moment a target gets a new subdomain.'
weight = 4
stack = ['Python', 'FastAPI', 'SQLModel', 'React', 'Docker']
repo = 'https://github.com/liuyc26/SubMon'
+++

**Problem.** In bug bounty, being *first* to a new asset matters as much as finding the bug.

**What I built.** A dashboard where you add targets, run or schedule scans (subfinder, dnsx, httpx), and see which subdomains are new or missing since the last scan, with page titles. A background worker sends a Discord notification whenever new subdomains appear.

**Result.** Four releases in about five weeks (Feb to Mar 2026): a dashboard, then scheduled scans and page titles, then multithreaded scanning (up to 8 workers) so large targets finish much faster, and a one-command Docker Compose setup.
