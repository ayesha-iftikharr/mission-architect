# Mission Architect

**Design a space mission, then fly it live.**

Built for the NASA Space Apps Challenge 2026, challenge: *Space Mission Design Game*.

**Play it:** https://github.com/ayesha-iftikharr/mission-architect
**Team:** Launch Window 
**Members** Ayesha Iftikhar, Zainab Sultan, Aima Hassan, Eman Waheed

---

## What it is

Mission Architect is a browser game where you design a complete robotic space mission and then run it turn by turn. Every choice has a price in money, mass, power or risk, so players feel why real mission designers rarely get a perfect answer.

## How to play

1. **Design.** Pick a destination, launch vehicle, spacecraft bus, propulsion system, communications system, orbit and science instruments. Stay inside the budget and the rocket's mass limit. A live diagram of your spacecraft updates as you choose.
2. **Launch.** The rocket and the orbit insertion can fail, so reliability matters.
3. **Fly.** Each turn, choose **Observe**, **Downlink** or **Recharge**. Observing collects data but drains the battery. Data only scores once it is sent to Earth.
4. **Handle surprises.** Random events (solar flares, antenna faults, battery faults, micrometeoroids, dust storms, discoveries) appear mid-flight. On higher difficulties a countdown timer forces a decision.
5. **Score.** Points come from data downlinked, plus a bonus for reaching the mission objective and for unspent budget. A report explains what happened and why.

Keyboard shortcuts during flight: **O**, **D**, **R** for the three modes, and **1**, **2**, **3** for event choices.

## What it teaches

| Concept | How the game shows it |
|---|---|
| Rocket equation (delta-v and Isp) | Propellant needed is calculated from the destination's velocity change and the engine's efficiency. A harder target or weaker engine means a much heavier launch. |
| Mass limits | The spacecraft plus its propellant must fit under the launch vehicle's capacity. |
| Power budget | Instruments draw power, solar output depends on distance from the Sun, and an empty battery causes a brownout. |
| Communications and data | A bigger antenna sends more per pass, but data collected and never sent is worth nothing. |
| Orbit trade-offs | Low orbits give sharper science but shorter life and less link time. High orbits give more link time and life but blurrier data and more radiation. |
| Risk and reserves | Unspent budget becomes a flight reserve for emergency fixes and upgrades. |

## Features

- Five destinations: the Moon, Mars, Venus, Europa and asteroid Bennu, each with its own objective
- Three difficulty levels (Cadet, Flight director, Mission chief)
- Live spacecraft diagram, resource ledger and flight dashboard
- Flight scene with animated downlinks, scans and launch
- Random events with timed decisions
- Upgrade shop paid from your flight reserve
- Mission report that explains the physics behind the result
- First-time tutorial and glossary
- Local list of your best missions
- Online team mode for up to four players (see below)

## Team mode

Up to four players can join one mission from their own devices. Each takes a role:

- **Mission planner:** destination, orbit, and the per-turn mode
- **Spacecraft engineer:** launch vehicle, bus, propulsion, and power or damage events
- **Scientist:** instruments and data events
- **Comms officer:** communications system and antenna events

One player presses **Host** and shares the room code, and the others press **Join**.

**Note:** online rooms need the game to be opened through its Claude link: [YOUR CLAUDE LINK, if public]. On the GitHub Pages version, solo play works fully, and the room buttons show a message instead.

## Data and sources

**Real figures**
- Launch vehicles: Falcon 9 (22,800 kg expended, about $70M list price, 99.5% success rate), Falcon Heavy (63,800 kg, about $97M to $150M) and Firefly Alpha (about 1,030 kg, about $15M)
- Europa Clipper benchmark (NASA/JPL): launch mass about 6,065 kg including about 2,750 kg of propellant, about 352 kg of instruments, about 600 W of solar power, and a lifecycle cost of about $5.2B

**Our estimates**
- Reliability of Falcon Heavy and Firefly Alpha

**Game values (simplified, not engineering data)**
- Spacecraft costs, bus and instrument stats, power use, events and scoring

**Sources**
- Falcon 9 data: https://orbitalradar.com/launch-vehicles/falcon-9
- AIAA Falcon vehicle guide: https://www.aiaa.org/vehicle-guide/vehicles/falcon
- Launch price comparison: https://greenlaunch.space/feeds/blog/cost-per-pound-space-launch
- NASA JPL Europa Clipper quick facts: https://www.jpl.nasa.gov/press-kits/europa-clipper/quick-facts/
- NASA JPL Europa Clipper spacecraft: https://jpl.nasa.gov/press-kits/europa-clipper/mission/spacecraft
- SpaceNews on Europa Clipper cost: https://spacenews.com/?p=507073

**NASA missions used as real-world analogs for the destinations:** Lunar Reconnaissance Orbiter, Mars Reconnaissance Orbiter, Europa Clipper, Magellan and OSIRIS-REx.

## Limitations

- This is a teaching game, not a mission planning tool. It does not model planetary flybys, detailed orbital mechanics or thermal design.
- Most numbers other than those listed above as real are simplified for gameplay.
- Team mode needs the Claude-hosted version, and its testing was limited.

## Run it locally

No install is needed. Download `index.html` and open it in a modern browser.

## Tech

Plain HTML, CSS and JavaScript in a single file, with no external libraries. Fonts load from Google Fonts, with system fonts as a fallback.

## Use of AI

This project was built with help from **Claude** (Anthropic), an AI assistant. Claude helped design the game, wrote the code, researched the real-world figures listed above. The visuals are drawn in code and contain no NASA logos or mission identifiers. I was testing it, giving commands where i felt a room for betterment. For example the idea of making players fly the mission live, because the first version felt boring, or the choice to add team roles. At first it was a very simple without any visual. But we managed to add visuals to make it next level. Its still a simple game but interactive one.

## Credits

Built by [Launch Window] for NASA Space Apps Challenge 2026.
This project is not affiliated with or endorsed by NASA.
