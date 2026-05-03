# RecMorph

# Early WIP — A community-driven reimplementation of the Rec Room servers, keeping Rec Room alive past June 1st, 2026.

# Note
This is my first time attempting a project of this scale, and reverse engineering stuff, so things may be rough around the edges. Bear with me!

# DISCORD: https://discord.gg/3w6SRMT7kS

**What is this?**

Rec Room is shutting down on June 1st, 2026. RestoRoom is an open-source effort to reverse engineer and reimplement the Rec Room server infrastructure so the community can keep playing after the lights go out.

This is a preservation project, built by fans, for fans.

**Status**

# This project is in very early development. Nothing is playable yet. We're currently in the research and reverse engineering phase.

Component
Network protocol research	In progress — 20 subdomains discovered
Account / auth server	Not started
Room server	Not started
Photon relay	Not started
Client patching / redirect	Not started
How it works (planned)

***Rec Room's backend consists of several systems we need to reimplement:***

REST API — account management, friends, inventory, room listings
Photon networking — real-time multiplayer via Photon SDK
Client redirect — patching the client to point at our servers instead of official ones

***Our approach:***

**1.** Sniff and document traffic between the Rec Room client and official servers

**2.** Reimplement each backend service

**3.** Patch or proxy the client to use our servers
