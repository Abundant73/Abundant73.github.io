---
layout: page
title: "Decoding the Drain: A Physics-Based Continuous-Time Model for Smartphone Battery Life Prediction"
description: Jan 2026
img: /assets/img/work - 001.png
importance: 1
category: work
related_publications: false
---

<style>
	h1.post-title {
		font-size: 2.0rem !important;
	}
	p.post-description,
	.post-description {
		font-size: 1.3rem !important;
	}
</style>



<div style="font-size: 1.2rem;">

	<h3>Summary</h3>
	<p><b>Can we mathematically predict smartphone battery life and identify the most effective power-saving interventions? </b>Despite over 6 billion smartphones in daily use, battery runtime remains frustratingly unpredictable—lasting a full workday under certain conditions yet draining before lunch under others. This study develops a rigorous physics-based framework to answer this question.</p>
	<p><b>Model Architecture. </b>This study formulated a continuous-time model based on coupled ordinary differential equations governing smartphone’s lithium-ion battery state of charge (SoC) dynamics. The framework integrates three subsystems: (1) electrochemical battery dynamics derived from lithium intercalation principles, (2) componentwise power decomposition modeling five subsystems (screen , CPU , network, GPS, and background processes) using intensity factor matrices, and (3) thermal-aging coupling incorporating Arrhenius degradation kinetics and SEI film growth. Meanwhile, time-to-empty is the zero point of the time equation with respect to SOC. </p>
	<p><b>Key Findings. </b>Model validation across typical scenarios (gaming, navigation, video watching) demonstrates strong predictive accuracy with relative errors under 8%. Sensitivity analysis reveals screen brightness and processor intensity as dominant drain factors, contributing 40-60% of total consumption in high-load scenarios. Critical insights include: (1) internal resistance surge below 20% SOC causes nonlinear performance degradation; (2) temperature elevation above 40°C doubles aging rate; (3) background tasks account for 15-25% consumption even during standby.</p>
	<p><b>Strategic Recommendations</b></p>
	<p><b>For Users: </b>Scenario-specific optimization includes reducing screen brightness by 30% during gaming (extending runtime 25%), pre-downloading offline maps for navigation (50% improvement), and selecting 720p video resolution (25% decoder power reduction). Long-term maintenance requires maintaining 20-80% SOC windows and avoiding charging above 30°C ambient temperature.</p>
	<p><b>For System Designers: </b>Implement adaptive power scheduling below 20% SOC, temperature-aware CPU throttling above 40°C, and machine learning-based usage pattern prediction for proactive resource allocation. Our model generalizes to laptops and power tools with subsystem reconfiguration.</p>

	<h3>Keywords</h3>
	<p>battery depletion model; SOC dynamics; multi-subsystem analysis; predictive power management</p>

	<br>

	<h3>Award</h3>
	<p><b>Honorable Mention</b> | 2026 Mathematical Contest in Modeling</p>

</div>

<br>

<div style="font-size: 1.3rem;">

	<p><b><em>Welcome to mail me for discussion!</em></b></p>

</div>




<br><br><br>