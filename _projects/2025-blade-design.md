---
layout: project
title: Wind Turbine Blade Design and Analysis
description: Advanced CAD and Fluid Analysis Project
technologies: [Autodesk Fusion]
image: /assets/images/blade_3.png
---

As part of the MAE 4272 Fluids and Heat Transfer Laboratory Class, our team designed and tested a set of custom wind turbine blades optimized for power output within the constraints of the department’s "big-blue" wind tunnel. The goal was to develop an efficient blade for a miniature wind turbine assembly that maintained structural integrity below a 2000 RPM limit and remained within a 6 in span and 2 in chord length. The project challenged us to balance aerodynamic performance and mechanical stress limits while developing a quantitative understanding of how design parameters affect torque, power extraction, and rotational speed.

Our design process began with aerodynamic modeling in QBlade, where we generated lift and drag polars across the expected Reynolds number range for various NACA profiles. Using a MATLAB blade-element model, we incorporated these polars to predict power and efficiency trends across several geometries. After comparing multiple configurations, we selected a NACA 4412 profile for its favorable lift-to-drag characteristics and moderate camber suitable for mid-range tip-speed ratios. The chosen design geometry was then modeled in CAD and printed out of Formlabs Resin.

![]({{ "/assets/images/power_curves.png" | relative_url }}){: .inline-image-r style="width: 250px"}

Testing was conducted in Cornell’s Big-Blue wind tunnel using a LabVIEW-controlled torque brake and pitot-tube pressure transducer system. We recorded torque and power at incremental torque-brake settings across a range of wind speeds, producing power curves for multiple operating conditions. The results confirmed expected physical trends, with power scaling approximately with the cube of velocity and peak efficiency shifting toward higher RPM with increasing wind speed. Discrepencies between observed and expected power outputs were most likely due to us realizing that the camber of our profile was incorrectly oriented with respect to the incoming wind velocity, which yielded lower power outputs for our wind speed range, however the general power and efficiency trends remained consistent with our analysis.

My contributions focused primarily on designing the blade geometry CAD model, where I decided which blade profiles I would efficiently loft over and made sure that the design was manufacturable and was consistent to the project guidelines. Future improvements of the design would focus on adjusting the camber to the prooer oritentation, refining the twist distribution to better match expected flow angles, and optimizing the design for higher tip-speed ratios through pitch and solidity adjustments.

![]({{ "/assets/images/turbine_2.JPG" | relative_url }}){: width="500px" }



