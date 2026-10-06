Lovable Preview- https://lovable.dev/preview/YWkQDkNHUTFap1Zg26wBJdCVsXY1pXgc

# UMBRA
### Human intent. Autonomous exploration. Knowing when to stop.

UMBRA is a lunar exploration simulator that asks: can AI understand
what a person means, act independently, and recognise when a mission
is unsafe?

Built for an OpenAI hackathon with GPT-6 Astra and Lovable, it puts
the user in command of a rover exploring the lunar south pole.

## How it works

Two GPT-6 Astra agents coordinate across a simulated Earth–Moon
communication delay:

- **Mission Control** interprets the commander’s goal and proposes a mission.
- **The rover agent** makes local decisions, explores, and reports its findings.
- **The commander** approves or rejects missions without manually driving.

Give UMBRA a plain-English goal:

> “Find water ice near the shadowed basin without risking the drill.”

Astra decides where to search, adapts when terrain becomes hazardous,
and refuses missions it cannot safely return from.

## What the demo demonstrates

- Turning human intent into exploration decisions.
- Inferring promising search areas from terrain and illumination.
- Rerouting when conditions differ from expectations.
- Explaining why an unsafe mission should not proceed.

The rover receives illumination data, but never the hidden simulated
ice map. It must reason about where to look.

## Real data and simulation

UMBRA uses lunar elevation and surface imagery distributed through
NASA’s Moon Trek portal. Illumination is calculated from the terrain.

Ice deposits, rover operations, and communication delay are simulated.
This is a concept prototype for exploring autonomous decision-making,
not a flight-ready rover system.

## Built with

- **Lovable:** mission-control UI and UX.
- **GPT-6 Astra:** mission planning and rover decision-making.
- **Lunar terrain data:** the environment for exploration.

Code applies the model’s chosen actions and calculates quantities
such as battery use, slope, distance, and mission risk.

## Why I built it

I wanted to explore what trustworthy autonomy looks like somewhere
human intervention cannot arrive immediately.

Completing a mission is only part of the challenge. Understanding
constraints, adapting to uncertainty, and knowing when to say no
are just as important.
