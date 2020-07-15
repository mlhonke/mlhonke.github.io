---
layout: single
title:  "Ferrofluid Simulation"
date:   2020-06-15 00:43:00 -0500
collection: projects
author_profile: true
toc: true
classes: wide
header:
    teaser: /assets/images/ferrofluid_front_small.jpg
---

Ferrofluids are a type of magnetic fluid. They have all the properties normally associated with fluids, such as viscosity, surface tension and density. However, the magnetic properties of ferrofluids allow for the velocity and static shape of the fluid to be manipulated using applied magnetic fields. My goal with this project was to simulate ferrofluids using an Eulerian (grid) based simulation. I wanted to especially capture the Rosensweig instability, a characteristic feature of ferrofluids. This phenomena results in ferrofluids displaying a pattern peaks on their surface when a sufficiently strong magnetic field is applied to the fluid.

# Examples
## Field Induced Motion
Water, initialized as a block, is used to fill a container. Simulation resolution is 60x60x60.
{% include video id="_pCorLhMZCM" provider="youtube" %}

## Rosensweig Instability
{% include video id="-VFo63_UEq8" provider="youtube" %}

# Technical Details

I first developed an [Eulerian fluid simulation]({% link _projects/2020-06-16-Eulerian-Fluid-Simulation.markdown %}) to serve as the base of my ferrofluid simulation. I then added the machinery to model a magnet, do magnetic potential solves, and then apply the resulting magnetic force to the fluid.

You can find out more about both my ferrofluid and fluid simulation techniques in my <a href="https://uwspace.uwaterloo.ca/bitstream/handle/10012/15859/Honke_Michael.pdf?sequence=3&isAllowed=y"> thesis</a>. You can see the code for my ferrofluid simulator on my <a href="https://github.com/mlhonke/simFerro">GitHub</a>, noting that all my general non-magnetic fluid code is a separate <a href="https://github.com/mlhonke/simFluid">repository</a>, which is included as an external static library by my ferrofluid simulator.
