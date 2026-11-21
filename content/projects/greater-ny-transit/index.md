+++
title = 'Greater NY Live Transit'
description = 'Live map of LIRR, Metro-North and NJ Transit trains and buses moving in and out of Manhattan, built to run at $0.'
weight = 1
stack = ['Python', 'FastAPI', 'Vercel', 'GitHub Actions', 'GTFS-realtime']
repo = 'https://github.com/liuyc26/greater-ny-transit'
demo = 'https://greater-ny-transit.vercel.app'
+++
<!-- DRAFT from the README. Please check and add why you built it / any results. -->

**Problem.** Commuter rail and bus feeds from the MTA and NJ Transit are rough: LIRR positions are often minutes old and NJ Transit train positions jump kilometers at a time, so plotting raw positions gives a jittery, misleading map.

**What I built.** A live map that snaps every vehicle onto its track and animates it toward the next stop's predicted arrival. Hover a train or bus to see its number, destination, next stop and delay. A daily GitHub Actions job rebuilds schedule data; a FastAPI app on Vercel serves live positions cached at the CDN, and NJ Transit data is fetched into one shared snapshot at most every 30 seconds so visitor traffic never multiplies upstream calls.

**Result.** Live at [greater-ny-transit.vercel.app](https://greater-ny-transit.vercel.app), running on free tiers.
