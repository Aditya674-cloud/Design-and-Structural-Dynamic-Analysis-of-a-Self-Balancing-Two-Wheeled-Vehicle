# 1. Introduction
## 1.1 Background

Self-balancing two-wheeled vehicles (commonly known as Segways) represent a class of inherently unstable mechanical systems, where the vehicle body must be actively controlled to remain upright — much like balancing a broomstick on your palm. Unlike conventional vehicles, which are passively stable, a self-balancing vehicle's mechanical structure, mass distribution, and dynamic behavior are tightly coupled with its control system. This means the mechanical design cannot be treated in isolation — every structural decision (frame stiffness, center of gravity location, mass distribution) directly influences the difficulty of the control problem, and vice versa.

This makes the self-balancing vehicle an excellent platform for demonstrating integrated mechanical engineering competency — spanning rigid body dynamics, structural analysis, and design validation — rather than any single narrow skill.

## 1.2 Motivation

Three factors motivate this project:

Technical depth: the system combines classical dynamics (Lagrangian mechanics), structural mechanics (modal/harmonic/fatigue analysis), and design validation (FEA) in one coherent problem — a genuine opportunity to apply theoretical coursework to a real design challenge.
Real-world relevance: self-balancing vehicles must survive realistic operating conditions — in this case, Indian road conditions, which are rougher and higher-frequency than smooth-road assumptions common in Western design references, requiring deliberate adjustment of analysis parameters (addressed in Section 12).
Engineering rigor as practice: this project deliberately documents not just final results, but the design process itself — including an early CG calculation error and its correction (Section 04) — reflecting how real engineering work involves iterative verification, not first-attempt perfection.

## 1.3 Problem Statement

Design and structurally validate the mechanical frame of a two-wheeled self-balancing vehicle capable of:

Supporting a rider of approximately 100 kg
Maintaining structural integrity under static loading, acceleration/braking-induced dynamic loading, and cornering loads
Surviving cyclic loading from motor-driven balancing corrections and road-induced vibration over a defined service life
Avoiding resonance within the expected operating frequency range (0–300 Hz, extended range justified by Indian road surface roughness)

## 1.4 Scope

This work covers the design and analysis phase of the vehicle's mechanical structure:

Included: CG determination, dynamic modeling (inverted pendulum, Lagrangian derivation), material selection, load case definition, static/modal/harmonic/fatigue FEA, design optimization based on analysis results
Explicitly excluded (at this stage): physical prototype fabrication and empirical/experimental validation — noted here for honesty, and identified as future work in Section 20

## 1.5 Objectives
Accurately determine system center of gravity and correct any errors in early estimates
Derive the governing dynamic equations of motion using Lagrangian mechanics and establish a linearized state-space model
Define realistic load cases based on expected operating conditions
Validate structural integrity through static, modal, harmonic, and fatigue FEA
Identify and address stress concentration risks and optimize frame design where needed
Consolidate all validation checks into a final design assessment
