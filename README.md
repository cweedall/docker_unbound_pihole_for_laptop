# Pi-hole with unbound (mobile)

Docker-compose configuration for pi-hole using unbound.  Aimed towards laptop using.

## Usage

1. Update OS / internet adapter DNS servers
  - Default
    1. `127.0.0.1`
    2. `1.1.1.1` (Cloudflare - change per your preference)
  - If using pi-hole at home/work already
    1. `[Pi-hole IP]` (e.g. `192.168.1.20`)
    2. `127.0.0.1`
    3. `1.1.1.1` (Cloudflare - change per your preference)

2. Navigate to `docker_unbound_pihole_for_laptop` project directory
from command line, run:

3. Run (3 options, depending on setup/preferences):

  -`docker-compose up` <sub>(allows monitoring and CTRL+C to terminate)</sub>

  -`docker-compose up -d` <sub>(daemon, running in background)</sub>

  -Run `docker_unbound_pihole_for_laptop` image in Docker Desktop application

4. Done!

## Overview

This is basically a **pi-hole** container running in **docker**.  It is meant to be run on a mobile device (e.g. a laptop) where you are likely to not be at home or at a friend's house who uses pi-hole already.  Because you don't want to lug around your Raspberry Pi, router running pi-hole, or equivalent thin client DNS server, this can be run locally and you get all the benefit of pi-hole!
