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
  Sep. 2024 – Present
</div>

<div class="section-heading">Overview</div>

Complex concave thin-walled metal components are critical for structural lightweighting in aerospace and automotive applications. However, traditional forming processes suffer from severe wrinkling instabilities and excessive localized wall thinning. 

This project establishes a novel **Gas-Liquid Low-Pressure Forming (GLLF)** technology for 6061 aluminum alloy tubes. By harnessing the high compressibility of the gas phase combined with flexible liquid support, the process achieves dynamic self-pressurization to overcome conventional forming boundaries.

<!-- 图片插槽 1：成形工艺原理与介质耦合示意图 -->
<div class="img-container">
  <img src="/images/gllf_principle.png" alt="GLLF Process Principle and Gas-Liquid Medium Interaction">
  <div class="img-caption">Fig. 1: Schematic illustration of the Gas-Liquid Low-Pressure Forming (GLLF) mechanism and dynamic pressurization concept.</div>
</div>

<div class="section-heading">Theory</div>

The deformation zone experiences a complex "tension-bending-compression" stress state. To predict instability limits and die-fitting requirements, analytical models were derived using plasticity mechanics and energy principles:

1. **Convex-Corner Die Fitting**: Evaluated via energy balance between plastic work and external loading ($p_c \propto \sigma_s, t/R$).
2. **Concave-Corner Attachment**: Modeled through stress superposition ($\sigma_\theta = \sigma_p + \sigma_d$) to prevent inward detachment.
3. **Straight-Wall Anti-Buckling Criterion**: Established using thin-plate stability theory under in-plane biaxial compression:
   $$p_{\text{cr, edge}} \ge \frac{F_d}{L \cdot t \cdot \sin\theta} - \frac{\pi^2 E}{12(1-\nu^2)} \left(\frac{t}{L}\right)^2$$

<!-- 图片插槽 2：理论力学模型与应力状态分析图 -->
<div class="img-container">
  <img src="/images/gllf_theory_model.png" alt="Analytical Model and Stress Distribution">
  <div class="img-caption">Fig. 2: Stress state decomposition and mechanical stability boundaries during concave corner fitting.</div>
</div>

<div class="section-heading">Methodology</div>

A combined experimental and numerical approach was deployed:

* **Finite Element Modeling**: Built full-scale models in **ABAQUS** with S4R shell elements and Swift strain-hardening laws ($\sigma = K\epsilon^n$).
* **Closed-Loop Co-Simulation**: Implemented a custom **Python script** dynamically coupling cross-sectional volume changes with instantaneous medium pressure increments across each solution step.
* **Experimental Validation**: Conducted forming tests on 6061-O aluminum tubes across $30^\circ$, $45^\circ$, and $60^\circ$ concave angles under varying initial gas ratios ($k = 0.6, 0.7$).

<!-- 图片插槽 3：实验设备、成形模具与工装架构 -->
<div class="img-container">
  <img src="/images/gllf_setup.png" alt="Experimental Machine Tooling and Dies">
  <div class="img-caption">Fig. 3: Modular forming die assembly, sealing system, and hydraulic experimental setup.</div>
</div>

<!-- 图片插槽 4：ABAQUS 有限元网格与 Python 动态耦合流程 -->
<div class="img-container">
  <img src="/images/gllf_simulation.png" alt="FEA Simulation Mesh and Python Algorithm Flowchart">
  <div class="img-caption">Fig. 4: ABAQUS finite element model, strain/stress contours, and Python-based dynamic P-V coupling flowchart.</div>
</div>

<div class="section-heading">Results and Discussion</div>

* **Wrinkling Suppression**: The nonlinear adaptive pressure trajectory (initial steady rise followed by exponential surge) successfully suppressed sidewall buckling during die closure.
* **Uniform Wall Thickness**: Shifted the fundamental deformation mode from tensile thinning to compressive accumulation, limiting maximum thinning rate within **5.5%**.
* **High Geometric Precision**: Global 3D profile deviation was strictly controlled within **0.5 mm**.

<!-- 图片插槽 5：成形管件实物图（不同角度/气液比对比） -->
<div class="img-container">
  <img src="/images/gllf_parts.png" alt="Formed Concave Aluminum Alloy Tubes">
  <div class="img-caption">Fig. 5: Macro-photographs of formed 6061-O aluminum alloy concave tubes under varying concave angles ($30^\circ, 45^\circ, 60^\circ$).</div>
</div>

<!-- 图片插槽 6：壁厚分布与三维扫描几何偏差测量图 -->
<div class="img-container">
  <img src="/images/gllf_thickness_deviation.png" alt="Wall Thickness Profile and 3D Deviation Map">
  <div class="img-caption">Fig. 6: Wall thickness distribution curves and 3D optical scanning deviation contours demonstrating high geometric accuracy.</div>
</div>

<div class="section-heading">Outlook</div>

Future work aims to extend the GLLF framework to ultra-high-strength materials (e.g., Titanium and Nickel-based alloys).