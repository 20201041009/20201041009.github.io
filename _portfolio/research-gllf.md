---
layout: single
title: "Gas-Liquid Low-Pressure Forming of Concave Thin-Walled Aluminum Alloy Tubes"
permalink: /portfolio/gllf-tube-forming/
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

<!-- 自动渲染 $...$ 行内公式与 $$...$$ 块级公式 -->
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
  Master's Thesis Project · Dalian University of Technology · Advisor: Prof. Zhubin He<br>
  Mar. 2026 – Sep. 2026
</div>

<div class="section-heading">Overview</div>

Complex concave thin-walled metal components are critical for structural lightweighting in aerospace and automotive applications. However, traditional forming processes suffer from severe wrinkling instabilities and excessive localized wall thinning. 

This project establishes a novel **Gas-Liquid Low-Pressure Forming (GLLF)** technology for 6061 aluminum alloy tubes. By harnessing the high compressibility of the gas phase combined with flexible liquid support, the process achieves dynamic self-pressurization to overcome conventional forming boundaries.

<!-- 图片插槽 1：试验装置与工艺原理图 -->
<div class="img-container">
  <img src="/images/gllf_setup.png" alt="GLLF Experimental Setup">
  <div class="img-caption">Fig. 1: Experimental setup and modular architecture for the Gas-Liquid Low-Pressure Forming process.</div>
</div>

<div class="section-heading">Theory</div>

The deformation zone experiences a complex "tension-bending-compression" stress state. To predict instability limits and die-fitting requirements, analytical models were derived using plasticity mechanics and energy principles:

1. **Convex-Corner Die Fitting**: Evaluated via energy balance between plastic work and external loading ($p_c \propto \sigma_s, t/R$).
2. **Concave-Corner Attachment**: Modeled through stress superposition ($\sigma_\theta = \sigma_p + \sigma_d$) to prevent inward detachment.
3. **Straight-Wall Anti-Buckling Criterion**: Established using thin-plate stability theory under in-plane biaxial compression:
   $$p_{\text{cr, edge}} \ge \frac{F_d}{L \cdot t \cdot \sin\theta} - \frac{\pi^2 E}{12(1-\nu^2)} \left(\frac{t}{L}\right)^2$$

<div class="section-heading">Methodology</div>

A combined experimental and numerical approach was deployed:

* **Finite Element Modeling**: Built full-scale models in **ABAQUS** with S4R shell elements and Swift strain-hardening laws ($\sigma = K\epsilon^n$).
* **Closed-Loop Co-Simulation**: Implemented a custom **Python script** dynamically coupling cross-sectional volume changes with instantaneous medium pressure increments across each solution step.
* **Experimental Validation**: Conducted forming tests on 6061-O aluminum tubes across $30^\circ$, $45^\circ$, and $60^\circ$ concave angles under varying initial gas ratios ($k = 0.6, 0.7$).

<!-- 图片插槽 2：ABAQUS 有限元仿真与 Python 动态耦合流程图 -->
<div class="img-container">
  <img src="/images/gllf_simulation.png" alt="Finite Element Simulation & Python Coupling">
  <div class="img-caption">Fig. 2: ABAQUS FEA model and Python-based pressure-volume dynamic coupling simulation flow.</div>
</div>

<div class="section-heading">Results and Discussion</div>

* **Wrinkling Suppression**: The nonlinear adaptive pressure trajectory (initial steady rise followed by exponential surge) successfully suppressed sidewall buckling during die closure.
* **Uniform Wall Thickness**: Shifted the fundamental deformation mode from tensile thinning to compressive accumulation, limiting maximum thinning rate within **5.5%**.
* **High Geometric Precision**: Global 3D profile deviation was strictly controlled within **0.5 mm**.

<!-- 图片插槽 3：成形管件实物与壁厚测量对比图 -->
<div class="img-container">
  <img src="/images/gllf_results.png" alt="Formed Component & Thickness Distribution">
  <div class="img-caption">Fig. 3: Comparison of formed concave aluminum alloy tubes and wall thickness distribution profiles.</div>
</div>

<div class="section-heading">Outlook</div>

Future work aims to extend the GLLF framework to ultra-high-strength materials (e.g., Titanium and Nickel-based alloys) and integrate real-time acoustic emission monitoring for adaptive pressure closed-loop control during high-speed industrial manufacturing.