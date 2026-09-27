\---

layout: single

title: "Gas-Liquid Low-Pressure Forming of Concave Thin-Walled Aluminum Alloy Tubes"

permalink: /research/gllf-tube-forming/

author\_profile: true

\---



<style>

&#x20; .project-subtitle {

&#x20;   text-align: center;

&#x20;   color: #666;

&#x20;   font-size: 1.05em;

&#x20;   margin-top: -15px;

&#x20;   margin-bottom: 25px;

&#x20; }

&#x20; .section-heading {

&#x20;   border-left: 4px solid #1a5fb4;

&#x20;   padding-left: 10px;

&#x20;   font-size: 1.4em;

&#x20;   font-weight: bold;

&#x20;   margin-top: 30px;

&#x20;   margin-bottom: 15px;

&#x20; }

&#x20; .img-container {

&#x20;   text-align: center;

&#x20;   margin: 20px 0;

&#x20; }

&#x20; .img-container img {

&#x20;   max-width: 100%;

&#x20;   border-radius: 6px;

&#x20;   box-shadow: 0 2px 8px rgba(0,0,0,0.12);

&#x20; }

&#x20; .img-caption {

&#x20;   font-size: 0.85em;

&#x20;   color: #666;

&#x20;   margin-top: 6px;

&#x20; }

</style>



<div class="project-subtitle">

&#x20; Master's Thesis Project · Dalian University of Technology · Advisor: Prof. Zhubin He<br>

&#x20; Mar. 2026 – Sep. 2026

</div>



<div class="section-heading">Overview</div>



Complex concave thin-walled metal components are critical for structural lightweighting in aerospace and automotive applications. However, traditional forming processes suffer from severe wrinkling instabilities and excessive localized wall thinning. 



This project establishes a novel \*\*Gas-Liquid Low-Pressure Forming (GLLF)\*\* technology for 6061 aluminum alloy tubes. By harnessing the high compressibility of the gas phase combined with flexible liquid support, the process achieves dynamic self-pressurization to overcome conventional forming boundaries.



<div class="img-container">

&#x20; <img src="/assets/images/gllf-experimental-setup.jpg" alt="GLLF Experimental Setup">

&#x20; <div class="img-caption">Fig. 1: Experimental setup and modular architecture for the Gas-Liquid Low-Pressure Forming process.</div>

</div>



<div class="section-heading">Theory</div>



The deformation zone experiences a complex "tension-bending-compression" stress state. To predict instability limits and die-fitting requirements, analytical models were derived using plasticity mechanics and energy principles:



1\. \*\*Convex-Corner Die Fitting\*\*: Evaluated via energy balance between plastic work and external loading ($p\_c \\propto \\sigma\_s, t/R$).

2\. \*\*Concave-Corner Attachment\*\*: Modeled through stress superposition ($\\sigma\_\\theta = \\sigma\_p + \\sigma\_d$) to prevent inward detachment.

3\. \*\*Straight-Wall Anti-Buckling Criterion\*\*: Established using thin-plate stability theory under in-plane biaxial compression:

&#x20;  $$p\_{\\text{cr, edge}} \\ge \\frac{F\_d}{L \\cdot t \\cdot \\sin\\theta} - \\frac{\\pi^2 E}{12(1-\\nu^2)} \\left(\\frac{t}{L}\\right)^2$$



<div class="section-heading">Methodology</div>



A combined experimental and numerical approach was deployed:



\* \*\*Finite Element Modeling\*\*: Built full-scale models in \*\*ABAQUS\*\* with S4R shell elements and Swift strain-hardening laws ($\\sigma = K\\epsilon^n$).

\* \*\*Closed-Loop Co-Simulation\*\*: Implemented a custom \*\*Python script\*\* dynamically coupling cross-sectional volume changes with instantaneous medium pressure increments across each solution step.

\* \*\*Experimental Validation\*\*: Conducted forming tests on 6061-O aluminum tubes across $30^\\circ$, $45^\\circ$, and $60^\\circ$ concave angles under varying initial gas ratios ($k = 0.6, 0.7$).



<div class="img-container">

&#x20; <img src="/assets/images/gllf-fem-coupling.jpg" alt="ABAQUS FE Modeling Framework">

&#x20; <div class="img-caption">Fig. 2: Volume-pressure-deformation coupling mechanism and Python-driven FE simulation.</div>

</div>



<div class="section-heading">Results and Discussion</div>



\* \*\*Wrinkling Suppression\*\*: The nonlinear adaptive pressure trajectory (initial steady rise followed by exponential surge) successfully suppressed sidewall buckling during die closure.

\* \*\*Uniform Wall Thickness\*\*: Shifted the fundamental deformation mode from tensile thinning to compressive accumulation, limiting maximum thinning rate within \*\*5.5%\*\*.

\* \*\*High Geometric Precision\*\*: Global 3D profile deviation was strictly controlled within \*\*0.5 mm\*\*.



<div class="section-heading">Outlook</div>



Future work aims to extend the GLLF framework to ultra-high-strength materials (e.g., Titanium and Nickel-based alloys) and integrate real-time acoustic emission monitoring for adaptive pressure closed-loop control during high-speed industrial manufacturing.

