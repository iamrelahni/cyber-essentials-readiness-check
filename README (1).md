# Cyber Essentials Readiness Check

A free, browser-based self-assessment that tells a UK SME how ready it is for Cyber Essentials under the Danzell question set (NCSC Requirements for IT Infrastructure v3.3), and what to fix first.

**Live tool:** https://iamrelahni.github.io/cyber-essentials-readiness-check/

## What it does

- 46 questions across scope and the five controls: firewalls, secure configuration, security update management, user access control, malware protection
- Plain English and Technical wording, switched with a toggle
- A traffic light per control, with automatic-fail conditions shown in their own row
- A prioritised action plan and a list of questions to send to your IT provider
- Three fictional example businesses to show it working

## How it scores

- **Automatic fails come first.** Missing 14-day patching (A6.4, A6.5), any cloud account without MFA (A7.14 to A7.17) and unsupported software are shown as blockers, whatever the overall score. "I don't know" on one of these shows as Unconfirmed, never green.
- **Each control** is red if a key question fails or there are three or more gaps or unknowns, amber for one or two, and green for none.
- **"Ready" only appears when every scored answer passes**, because Cyber Essentials is pass or fail on every requirement.

## Privacy

Everything runs in the browser. Answers are saved in local storage on the user's own device and are never sent anywhere.

## Running it

It is a single file with no build step. Open `index.html` in a browser, or host it with GitHub Pages.

## Status and limits

Version 1.1. Every question and scoring rule was reviewed against the NCSC v3.3 requirements document on 11 November 2026. Automatic-fail status is taken from IASME partner guidance; unsupported software is treated as an automatic fail as a cautious choice, as not every source lists it.

Not covered in this version:

- Sub-set scoping (certifying only a segregated part of an organisation)
- The extra requirements for organisations that use application allow-listing instead of anti-malware
- Cyber Essentials Plus technical testing

**This is not a Cyber Essentials assessment or certification**, and it is not affiliated with the NCSC or IASME. A good result does not guarantee a pass. Certification is only available through an IASME certification body. The tool is provided as is, for guidance only; check the official requirements before you apply.

## About

Built by Leo Greathead with AI assistance (Claude). The spec, scoring decisions and review against the source document are mine.
