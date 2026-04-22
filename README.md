# Endogenous Growth Simulation Interactive Romer R&D Model Dashboard

## Description
The simulation represents the Romer endogenous growth model, whereby an economy with given total labor (***L***) generates workers for the production (***L<sub>Y</sub>***) and research and development (**R&D**, ***L<sub>R</sub>***) sectors. Capital and labor are deployed by firms in production to generate output. ***L<sub>R</sub>*** generates new ideas that promote sustained growth, as opposed to the Solow model where technology is exogenous. Users can manipulate major parameters in real time to observe the equilibrium labor allocation, including: R&D productivity (***θ***), Markup (***μ***), Interest rate (***r***), Capital intensity (***α***), and Total Labor (***L***).

---


## How the Simulation Works <br>
The simulation replicates the "bridge" created in the paper to solve for the market equilibrium of R&D labor, which is typically considered too complex for undergraduate studies.

 ➤ **Labor Allocation Logic**: The core of the code divides the total labor force ($L$) into two sectors: Production Labor (***L<sub>Y</sub>***) and R&D Labor (***L<sub>R</sub>***).

 ➤ **Equilibrium Determination:** The code calculates the equilibrium based on the condition where the cost of R&D (wages) equals the value of a new invention (the present value of future monopolistic profits).

 ➤ **Growth Rate Calculation:** The final growth rate (***g<sup>*</sup>***) is derived from the R&D labor multiplied by productivity: ***g<sup>*</sup>*** = ***θ******L<sub>R</sub>***. The simulation specifically uses the formula:

$$g^* = \theta L - \frac{1-\alpha}{\alpha} \left( \frac{\mu}{\mu - 1} \right) r$$

where ***α*** is capital share and ***r*** is the interest rate.

 ➤ **Output Trajectory:** It uses this growth rate to project the path of Output (**_Y_**) over time on a log scale, comparing it against a baseline growth rate (typically 2%)

 ➤ **Parameters:** The parameters used in the simulation are the following 
   - ***θ***: R&D Productivity
   - ***L***: Total Labor
   - ***α***: Capital Share
   - ***μ***: Market Markup
   - ***r***: Interest Rate
   - ***T***: Time Horizon (Years)

---


## Actors of the Simulation Design: <br>
➤ **Laborers:** The total workforce is split into two groups which are: <br>
    -  **Production Workers:** These are the people who make the things we use every day. <br>
    -  **Researchers (R&D):** The Researchers are the people who come up with ideas and designs for things.

➤ **Monopolists:** Intermediate firm owners who buy blueprints and use their market power (markup) to earn profits, which fund the R&D.

---

