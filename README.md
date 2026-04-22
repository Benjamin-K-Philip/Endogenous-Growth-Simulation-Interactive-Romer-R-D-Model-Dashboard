# Endogenous Growth Simulation Interactive Romer R&D Model Dashboard

## Description
The simulation represents the Romer endogenous growth model, whereby an economy with given total labor (***L***) generates workers for the production (***L<sub>Y</sub>***) and research and development (**R&D**, ***L<sub>R</sub>***) sectors. Capital and labor are deployed by firms in production to generate output. ***L<sub>R</sub>*** generates new ideas that promote sustained growth, as opposed to the Solow model where technology is exogenous. Users can manipulate major parameters in real time to observe the equilibrium labor allocation, including: R&D productivity (***θ***), Markup (***μ***), Interest rate (***r***), Capital intensity (***α***), and Total Labor (***L***).

---

**Endogenous Growth Simulation (Romer Model)**

The core economic logic defines the long-run growth rate (***g<sup>*</sup>***) and the equilibrium labor allocation between the production sector (***L<sub>Y</sub>***) and the R&D sector (***L<sub>R</sub>***). The output trajectory (***Y<sub>t</sub>***) grows exponentially over time (***t***) based on this endogenously determined growth rate.

**Core Equations:**
* **Growth Rate (***g<sup>*</sup>***):** ***g<sup>*</sup>*** = ***θL*** - [ (1 - ***α***) / ***α*** ] * [ ***μ*** / (***μ*** - 1) ] * ***r***
* **Production Labor (***L<sub>Y</sub>***):** ***L<sub>Y</sub>*** = [ (1 - ***α***) / (***αθ***) ] * [ ***μ*** / (***μ*** - 1) ] * ***r***
* **R&D Labor (***L<sub>R</sub>***):** ***L<sub>R</sub>*** = ***L*** - ***L<sub>Y</sub>***
* **Output Trajectory:** ***Y<sub>t</sub>*** = ***Y<sub>0</sub>***(1 + ***g<sup>*</sup>***)<sup>***t***</sup>

**Parameters:**
* ***θ***: R&D Productivity
* ***L***: Total Labor
* ***α***: Capital Share
* ***μ***: Market Markup
* ***r***: Interest Rate
* ***T***: Time Horizon (Years)
