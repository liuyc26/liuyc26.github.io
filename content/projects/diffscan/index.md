+++
title = 'diffscan'
description = 'Secret scanner for git repositories: 33 detection rules plus entropy checks to catch leaked API keys and credentials in commit diffs.'
weight = 3
stack = ['Python', 'FastAPI', 'SQLAlchemy', 'PostgreSQL', 'Docker']
repo = 'https://github.com/liuyc26/diffscan'
+++
<!-- DRAFT from the README. Please check and add why you built it / any results. -->

**Problem.** API keys, tokens and private keys end up in git history, and once pushed they are hard to spot by hand.

**What I built.** A lightweight scanner with 33 named rules (AWS, GCP, Azure, GitHub, Stripe, Slack, PEM keys, JWTs, database URLs and more) plus entropy detection for secrets that evade rules. It scans the latest commit, the last N commits or full history on any branch, can monitor repos in the background, masks matched values, and lets you resolve false positives.

**Result.** 80 automated tests; runs locally on SQLite or with Docker Compose on PostgreSQL.
