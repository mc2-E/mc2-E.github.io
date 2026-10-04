---
layout: page
title: "Molten-Salt Corrosion: Comprehensive Implementation"
description: Configurable Cr-only and Cr–Fe reaction kinetics with analytical alloy transport.
permalink: /research/projects/molten-salt-corrosion/comprehensive-implementation/
nav: false
nav_parent: /about/
---

<style>
.project-breadcrumb {font-size:.9rem;margin-bottom:1.25rem;overflow-wrap:anywhere;}
.implementation-grid {display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1rem;margin:1.5rem 0;}
.implementation-card {padding:1.25rem;border:1px solid var(--global-divider-color,#d7d0d0);border-top:4px solid var(--global-theme-color,#500000);border-radius:8px;background:var(--global-card-bg-color,var(--global-bg-color,#fff));}
.implementation-card h2 {font-size:1.25rem;margin:.25rem 0 .75rem;line-height:1.3;}
.implementation-card p {margin-bottom:.8rem;}
.project-links {display:flex;flex-wrap:wrap;gap:.5rem 1rem;margin-top:1rem;}
.project-links a {font-weight:500;}
@media(max-width:700px) {.implementation-grid {grid-template-columns:1fr}}
</style>

<nav class="project-breadcrumb" aria-label="Breadcrumb"><a href="{{ '/about/' | relative_url }}">Research</a> / <a href="{{ '/research/projects/' | relative_url }}">Projects</a> / <a href="{{ '/research/projects/molten-salt-corrosion/' | relative_url }}">Molten-salt corrosion</a> / Comprehensive implementation</nav>

This unified explorer extends the focused Cr-only studies to **configurable Cr-only or Cr+Fe dissolution and deposition**. It combines analytical spatial transport with numerically solved, nonlinear activity-based Butler–Volmer interface kinetics. Use it to test how reaction assumptions, thermodynamic reference gaps and finite or maintained salt chemistry change element redistribution and net metal transfer.

<div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/comprehensive-implementation/configurable-kinetics/' | relative_url }}">Open the configurable corrosion explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/comprehensive-implementation/configurable-kinetics/' | relative_url }}?bath=finite">Start with finite-bath mixed potential →</a><a href="{{ '/research/projects/molten-salt-corrosion/comprehensive-implementation/configurable-kinetics/index.html' | relative_url }}" download="Configurable_BV_Corrosion_Explorer.html">Download the offline HTML</a></div>

## What you can explore

- **Electrical conditions:** prescribed actual Cr overpotential, prescribed common electrode potential, or mixed potential with maintained chemistry or finite bath inventories.
- **Reaction kinetics:** Cr-only or Cr+Fe exchange, reference exchange currents, transfer coefficients, and source-informed, linear, constant or custom activity-power prefactors.
- **Reference states and chemistry:** separate equilibrium-reference gaps, maintained or initial salt activity ratios, and a display-reference offset that changes reported potentials without changing the physics.
- **Finite bath:** separate initial dissolved Cr and Fe inventories, shared HF/H₂ capacity, evolving activities, and a zero-partial-current equilibrium. All the same metal-reaction and activity-law controls remain available.
- **Alloy transport:** transport length, initial/far vacancy supersaturation and a Cr tracer-diffusivity multiplier.
- **Results:** element and vacancy profiles with interface zoom, signed Cr/Fe and net transfer, time histories through two years, independent stationary states or finite-bath equilibrium, and frozen-state polarization plots. CSV and parameter exports are included.

## A suggested starting point

Open the default 100 µm, 700 °C maintained-chemistry case. Compare Cr+Fe with Cr-only, then vary one parameter at a time. Examine both individual element transfer and net removal: Fe deposition can offset Cr dissolution. Then select **Mixed potential — finite bath** and inspect the **Bath chemistry** tab. Follow dissolved Fe consumption alongside HF/H₂ evolution. Distinguish the two-year transient from the independent endpoint: finite-bath equilibrium has zero active partial currents, whereas maintained chemistry can sustain stationary transfer.

## Scope and assumptions

Bulk transport coefficients are evaluated at the chosen initial/far-alloy reference and held constant during each trajectory; surface thermodynamic activities and reaction kinetics remain nonlinear. The transient calculation is semianalytical, using analytical diffusion responses with numerical time integration and boundary solves. It does not run MOOSE.

The kinetic mapping is a conditional adaptation of source measurements, and adjustable prefactors are sensitivity choices. A converged stationary root does not by itself establish stability, uniqueness or attainment within two years. Equivalent metal transfer is not wall recession. The explorer’s **Model** tab explains the equations, evidence and limitations.

The finite-bath default uses equal initial effective dissolved Cr and Fe inventories (0.188507 mol/m² each) and a shared capacity of 1.885074 mol/m². These are controlled comparison inputs, not a measured salt composition. Activity ratios scale with the remaining inventories; no spatial salt transport or gas equation of state is solved. The fixed far-alloy reservoir remains available. Positive kinetic-prefactor changes affect the approach to equilibrium, while the equilibrium itself depends on thermodynamics and inventories.

The earlier focused Cr-only tools remain available under the [Simple Implementation]({{ '/research/projects/molten-salt-corrosion/simple-implementation/' | relative_url }}).

The explorer runs in a modern browser without sign-in or installation. For offline use, save the HTML and open it locally; calculations and plots work offline, while optional literature links require internet access.

[← Molten-salt project]({{ '/research/projects/molten-salt-corrosion/' | relative_url }})

