# Source Catalog

This file tracks realistic source candidates before they are promoted into BNTL Core · Paradox Engine.

## Candidate Source Families

- NOAA SWPC space weather products
- USGS earthquake feeds
- NWS weather alerts
- NASA DONKI / space weather candidates
- NASA GCN notices
- LIGO / Virgo / KAGRA public notices where available
- Market provider candidates
- News/social provider candidates
- Device sensor candidates
- Manual operator input

## Promotion Flow

Planned → Sample UI Data → Endpoint Verified → EventEnvelope Ready → Safety Checked → Director Console Ready → Live Connected

## Required Review

- Official source identified
- Endpoint family documented
- Auth method documented
- License reviewed
- Rate limits reviewed
- EventEnvelope mapping drafted
- Error handling drafted
- Degraded mode drafted
- Provenance plan drafted
