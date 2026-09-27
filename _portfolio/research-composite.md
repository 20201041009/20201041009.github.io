---
layout: single
title: "Development of Large-Sized Integrated Thermoplastic Composite Structure"
permalink: /portfolio/composite-structure/
author_profile: true
---

<style>
  .project-subtitle {
    text-align: center;
    color: #666;
    font-size: 1.05em;
    margin-top: -15px;
    margin-bottom: 25px;
  }
  .section-heading {
    border-left: 4px solid #1a5fb4;
    padding-left: 10px;
    font-size: 1.4em;
    font-weight: bold;
    margin-top: 30px;
    margin-bottom: 15px;
  }
  .my-contribution-box {
    background-color: #f8f9fa;
    border: 1px solid #e9ecef;
    border-left: 4px solid #28a745;
    padding: 15px 20px;
    border-radius: 4px;
    margin: 20px 0;
  }
  .img-container {
    text-align: center;
    margin: 20px 0;
  }
  .img-container img {
    max-width: 100%;
    border-radius: 6px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.12);
  }
  .img-caption {
    font-size: 0.85em;
    color: #666;
    margin-top: 6px;
  }
</style>

<!-- 自动渲染公式支持 -->
<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

<div class="project-subtitle">
  Key R&D Project · Dalian University of Technology<br>
  Jan. 2025 – April. 2026
</div>

<div class="section-heading">Overview</div>

Thermoplastic composites offer superior fracture toughness, recyclable properties, and rapid thermoforming capabilities compared to traditional thermosets. This project focuses on the design, thermal-mechanical mold tooling, and manufacturing process optimization of large-scale integrated thermoplastic composite structural components.

<!-- 图片插槽 1：大型热压成形模具与工装平台 -->
<div class="img-container">
  <img src="/images/composite_molds.png" alt="Large-scale Thermoforming Mold and Equipment Setup">
  <div class="img-caption">Fig. 1: Large-scale thermoforming mold tooling and high-capacity hydraulic press setup at Dalian University of Technology.</div>
</div>

<div class="section-heading">My Contribution</div>

<div class="my-contribution-box">
  <strong>Key Responsibilities & Individual Deliverables:</strong>
  <ul>
    <li><strong>Thermoforming Mold Design</strong>: Independent CAD/UG modeling of composite thermoforming tooling and dynamic thermal expansion gap calculations.</li>
    <li><strong>Modular Insert Prototyping</strong>: Designed and 3D-printed custom modular inserts for rapid mold reconfiguration during experimental layup iterations.</li>
    <li><strong>Process Setup & Execution</strong>: Assembled thermoforming units, established temperature/pressure holding profiles, and performed post-forming dimensional inspection.</li>
  </ul>
</div>

<div class="section-heading">Theory</div>

The thermoforming behavior of continuous fiber-reinforced thermoplastics involves non-isothermal crystallization kinetics and temperature-dependent viscoelastic matrix flow. Dimensional stability is dictated by anisotropic thermal shrinkage ($\alpha_{L} \ll \alpha_{T}$) and inter-ply consolidation pressure distribution during the cooling phase.

<div class="section-heading">Methodology</div>

1. **Tooling & Inserts Optimization**: Designed thermoforming mold components in Siemens UG/NX and utilized FDM 3D printing for rapid modular insert fabrication.
2. **Thermal-Mechanical Co-Simulation**: Performed transient heat transfer and consolidation pressure field modeling in ABAQUS.
3. **Consolidation Experiments**: Conducted high-temperature press consolidation tests using optimized heating rate, dwell pressure, and controlled cooling paths.

<!-- 图片插槽 2：热压及压弯实验过程 -->
<div class="img-container">
  <img src="/images/composite_experiments.png" alt="Thermoforming and Bending Process">
  <div class="img-caption">Fig. 2: Experimental procedures for flat plate thermoforming, 145° angle press bending, and section profile consolidation.</div>
</div>

<div class="section-heading">Results and Discussion</div>

* **Full-Scale Flat Panel Consolidation**: Successfully fabricated extra-large thermoplastic composite panels ($3520 \text{ mm} \times 920 \text{ mm}$) with excellent surface quality and zero macro-voids.
* **Complex Structural Elements**: Achieved precise forming of integrated $\Omega$-shaped stiffening beams and $145^\circ$ press-bent structural ribs with uniform flange thickness ($50 \text{ mm}$).
* **Rapid Tooling Reconfiguration**: 3D-printed modular inserts reduced tooling modification lead times by **60%**, enabling fast physical validation of complex rib geometries.

<!-- 图片插槽 3：成形实物件（平板、大尺寸梁及弯曲件） -->
<div class="img-container">
  <img src="/images/composite_results.png" alt="Formed Thermoplastic Composite Components">
  <div class="img-caption">Fig. 3: Consolidated thermoplastic composite specimens, including $3520\text{ mm}$ flat panels, $\Omega$-stiffeners, and 145° angled profiles.</div>
</div>

<!-- 图片插槽 4：装配与焊接组装应用 -->
<div class="img-container">
  <img src="/images/composite_assembly.png" alt="Assembly and Structural Integration">
  <div class="img-caption">Fig. 4: Integration and welding assembly of large thermoplastic panel structures (hangar, chimney wall, and side panel units).</div>
</div>

<div class="section-heading">Outlook</div>

Future investigations will focus on automated fiber placement (AFP) coupling and ultrasonic consolidation testing for automated, high-throughput manufacturing of primary aerospace load-bearing parts.