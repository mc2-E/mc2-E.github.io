---
layout: page
title: "Molten-Salt Corrosion: Simple Implementation"
description: Five focused Cr-only analytical explorers, supporting reports and offline downloads.
permalink: /research/projects/molten-salt-corrosion/simple-implementation/
nav: false
nav_parent: /about/
---

<style>
.project-breadcrumb {font-size:.9rem;margin-bottom:1.25rem;}
.project-lead {font-size:1.08rem;line-height:1.65;}
.project-tools {display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1rem;margin:1.5rem 0;}
.project-tool {padding:1.25rem;border:1px solid var(--global-divider-color,#d7d0d0);border-radius:8px;background:var(--global-card-bg-color,var(--global-bg-color,#fff));}
.project-tool:first-child {grid-column:1/-1;border-left:4px solid var(--global-theme-color,#500000);}
.project-tool h3 {font-size:1.18rem;margin:.3rem 0 .6rem;line-height:1.3;}
.project-tool p {margin-bottom:.7rem;}
.project-eyebrow {font-size:.8rem;font-weight:600;letter-spacing:.025em;}
.project-links {display:flex;flex-wrap:wrap;gap:.5rem 1rem;align-items:center;margin-top:1rem;}
.project-links a {font-weight:500;}
.project-note {padding:1rem 1.25rem;border-left:3px solid var(--global-theme-color,#500000);background:var(--global-code-bg-color,#f6f3f3);margin:1.5rem 0;}
@media(max-width:700px) {.project-tools {grid-template-columns:1fr}.project-tool:first-child {grid-column:auto}}
</style>

<nav class="project-breadcrumb" aria-label="Breadcrumb"><a href="{{ '/about/' | relative_url }}">Research</a> / <a href="{{ '/research/projects/' | relative_url }}">Projects</a> / <a href="{{ '/research/projects/molten-salt-corrosion/' | relative_url }}">Molten-salt corrosion</a> / Simple implementation</nav>

Start here for focused studies of **Cr-only selective dissolution** in a one-dimensional Fe–Ni–Cr–vacancy alloy. The five explorers separate the effects of transport length, Cr diffusivity, vacancies, imposed overpotential and finite versus maintained salt chemistry. Supporting reports and offline packages accompany the tools.

The bulk transport coefficients are evaluated at the selected reference state and held fixed during each calculation. The surface laws differ among the tools, from a linear reaction benchmark to nonlinear activity-based mixed-potential kinetics; each explorer states its own assumptions. This collection is useful for understanding individual mechanisms and building analytical benchmarks.

For configurable Cr-only or Cr+Fe exchange and user-adjustable Butler–Volmer kinetics, use the [Comprehensive Implementation]({{ '/research/projects/molten-salt-corrosion/comprehensive-implementation/' | relative_url }}).

## Analytical explorers

Start with **Cr diffusivity and vacancy effects** for a comparison across all three interface conditions. The other tools examine individual mechanisms and targeted questions in greater detail.

<div class="project-tools">
<section class="project-tool" aria-labelledby="tool-diffusivity">
  <span class="project-eyebrow">Start here</span>
  <h3 id="tool-diffusivity">Cr diffusivity and vacancy effects</h3>
  <p><strong>How much do uncertain Cr diffusivity and vacancy concentrations change corrosion?</strong></p>
  <p>Compare prescribed overpotential, a finite bath, and maintained chemistry. Change Cr tracer diffusivity, the initial/far vacancy reference, or both; examine profiles and rates from 1 hour to two years and the final state.</p>
  <p>Includes the diffusivity evidence report and numerical evidence table.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/diffusivity/' | relative_url }}">Open explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/downloads/Cr_Diffusivity_Analytical_Study.zip' | relative_url }}" download>Offline ZIP</a></div>
</section><section class="project-tool" aria-labelledby="tool-prescribed-potential">
  <span class="project-eyebrow">Interface condition</span>
  <h3 id="tool-prescribed-potential">Prescribed-overpotential response</h3>
  <p><strong>How do size, vacancies and imposed overpotential affect the response?</strong></p>
  <p>Explore steady and transient Ni, Cr and vacancy profiles, size effects, removal rates, polarization curves and differential resistance. This benchmark uses a concentration-linear surface reaction.</p>
  <p>Includes the parameter-sensitivity report with electrochemical plots.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/prescribed-potential/' | relative_url }}">Open explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/downloads/Prescribed_Potential_Analytical_Explorer.zip' | relative_url }}" download>Offline ZIP</a></div>
</section><section class="project-tool" aria-labelledby="tool-mixed-potential">
  <span class="project-eyebrow">Environmental feedback</span>
  <h3 id="tool-mixed-potential">Finite bath versus maintained chemistry</h3>
  <p><strong>What changes when the salt chemistry evolves or is maintained?</strong></p>
  <p>Compare current-balanced mixed potential in a finite closed bath and a maintained reservoir. Follow alloy profiles, accumulated removal, bath chemistry, equilibrium-potential shifts and Evans diagrams.</p>
  <p>Analytical spatial transport with numerically integrated nonlinear interface kinetics.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/mixed-potential/' | relative_url }}">Open explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/downloads/Mixed_Potential_Analytical_Explorer.zip' | relative_url }}" download>Offline ZIP</a></div>
</section><section class="project-tool" aria-labelledby="tool-target-rate">
  <span class="project-eyebrow">Inverse calculation</span>
  <h3 id="tool-target-rate">Work backward from a target rate</h3>
  <p><strong>Which parameters would be needed to reach a selected steady removal rate?</strong></p>
  <p>Specify a target Cr-equivalent removal rate and solve for vacancy supersaturation, Cr tracer diffusivity, or prescribed overpotential. Includes maintained-chemistry mixed potential and identifies targets outside the selected search range.</p>
  <p>Positive steady-rate targets apply to prescribed or maintained-chemistry conditions.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/target-rate/' | relative_url }}">Open explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/downloads/Target_Rate_Analytical_Explorer.zip' | relative_url }}" download>Offline ZIP</a></div>
</section><section class="project-tool" aria-labelledby="tool-diffusion-interface-control">
  <span class="project-eyebrow">Rate-limiting mechanisms</span>
  <h3 id="tool-diffusion-interface-control">Diffusion versus interface control</h3>
  <p><strong>Where does diffusion or the interface contribute most of the resistance?</strong></p>
  <p>Sweep vacancy supersaturation or the Cr tracer-diffusivity multiplier. Locate 90% diffusion control, equal resistance, and 90% interface control, and relate limiting transfer capacities to the overall removal rate.</p>
  <p>Prescribed-overpotential benchmark; the extended sweep is a mathematical sensitivity range.</p>
  <div class="project-links"><a href="{{ '/research/projects/molten-salt-corrosion/simple-implementation/diffusion-interface-control/' | relative_url }}">Open explorer →</a><a href="{{ '/research/projects/molten-salt-corrosion/downloads/Diffusion_Interface_Control_Explorer.zip' | relative_url }}" download>Offline ZIP</a></div>
</section>
</div>

## Reports and offline access

- [Cr diffusivity in 316-like alloys: evidence and uncertainty (PDF)]({{ '/research/projects/molten-salt-corrosion/reports/Cr_Diffusivity_Uncertainty.pdf' | relative_url }}) · [Evidence table (CSV)]({{ '/research/projects/molten-salt-corrosion/data/Diffusivity_973K_Evidence.csv' | relative_url }})
- [Prescribed-overpotential parameter sensitivity and electrochemical plots (PDF)]({{ '/research/projects/molten-salt-corrosion/reports/Prescribed_Analytical_Sensitivity.pdf' | relative_url }})
- [Download all five analytical tools and both reports (ZIP)]({{ '/research/projects/molten-salt-corrosion/downloads/Molten_Salt_Analytical_Tools.zip' | relative_url }})

The explorers run directly in a modern browser, with no sign-in or software installation. For offline use, extract a ZIP and open **Start_Here.html**. The calculations work offline; external literature links require internet access. Each explorer provides its own CSV or parameter exports.

## Reading the predictions

The plotted rates are **Cr-equivalent removal rates**, calculated from chromium transfer per unit area. They are not direct predictions of wall recession or depletion depth. The models use a fixed planar domain and fixed far-alloy composition. Their bulk transport coefficients are evaluated at the chosen reference state and held constant during each analytical trajectory.

Prescribed overpotential holds the actual Cr driving overpotential fixed. The two mixed-potential conditions instead solve anodic–cathodic current balance: the finite bath evolves chemically, while maintained chemistry holds the salt activities fixed. The prescribed benchmark also uses a different, linear surface law; its contrast with the mixed-potential tools includes that distinction. Each explorer documents its equations, parameter ranges and assumptions.

[← Molten-salt project]({{ '/research/projects/molten-salt-corrosion/' | relative_url }})

