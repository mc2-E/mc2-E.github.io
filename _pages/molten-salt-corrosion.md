---
layout: page
title: Molten-Salt Corrosion
description: Alloy transport, interface kinetics and salt chemistry, from focused benchmarks to configurable reaction models.
permalink: /research/projects/molten-salt-corrosion/
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

<nav class="project-breadcrumb" aria-label="Breadcrumb"><a href="{{ '/about/' | relative_url }}">Research</a> / <a href="{{ '/research/projects/' | relative_url }}">Projects</a> / Molten-salt corrosion</nav>

Our molten-salt corrosion project investigates how alloy diffusion, thermodynamic interactions, vacancy transport and interfacial electrochemistry combine to control selective dissolution. The broader research connects modeling with experiments on 316H stainless steel for molten-salt energy systems.

Explore the project through two implementations. Both use a one-dimensional alloy representation and analytical or semianalytical transport calculations, primarily at 700 °C.

<div class="implementation-grid">
<section class="implementation-card" aria-labelledby="simple-title">
  <h2 id="simple-title">Simple Implementation</h2>
  <p>Five focused explorers for Cr-only dissolution: diffusivity and vacancy effects, prescribed overpotential, finite versus maintained baths, target-rate calculations, and diffusion versus interface control.</p>
  <p>Begin here to isolate mechanisms and compare benchmarks. Includes supporting reports and offline downloads.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/' | relative_url }}">Explore the simple implementation →</a></div>
</section>
<section class="implementation-card" aria-labelledby="comprehensive-title">
  <h2 id="comprehensive-title">Comprehensive Implementation</h2>
  <p>A unified, configurable explorer for Cr-only or Cr+Fe dissolution and deposition. Vary activity-dependent kinetics, equilibrium-reference gaps, bath activities and electrical constraints within one model.</p>
  <p>Compare prescribed Cr overpotential, prescribed electrode potential and maintained-chemistry mixed potential, with profiles, time histories and electrochemical plots.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/comprehensive-implementation/' | relative_url }}">Explore the comprehensive implementation →</a></div>
</section>
</div>

## Reading the predictions

These tools hold the bulk transport coefficients fixed at the selected reference state. They provide analytical benchmarks and semianalytical sensitivity studies; they are not the full evolving-coefficient MOOSE model. “Comprehensive” describes the configurable reaction choices in the newer explorer.

Rates represent **equivalent metal transfer per unit area**, not direct wall recession or depletion depth. The simple tools report Cr-equivalent removal; the comprehensive explorer also separates signed Cr and Fe transfer from net metal removal. Assumptions and applicable parameter ranges are documented within each tool.

[← All research projects]({{ '/research/projects/' | relative_url }})
