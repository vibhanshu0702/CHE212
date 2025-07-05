# CHE212 Innovation Project: Thermal Resistance in Metal Rod Combinations

## Team Members
- Anshika Agrawal  
- Tanvi Manhas  
- Vibhanshu  
- Sahil Kumar  

## Objective
The objective of this project is to experimentally determine the thermal resistance of metal rod combinations and compare the results with theoretical values. Additionally, a transient analysis was conducted to study the temperature response over time.

## Materials Used
- Metal rods (Copper, Aluminium, Iron)  
- Power source and power display  
- Arduino for data logging  
- Temperature sensors (T1, T2, T3)  
- Teflon insulation

## Experimental Setup
Three series combinations of metal rods were used:
- Copper – Aluminium  
- Aluminium – Iron  
- Iron – Copper  

Each setup consisted of two rods joined together, with temperature sensors placed at the hot end, the junction, and the cold end. A constant heat source was applied, and data was logged at regular intervals until steady-state was achieved.

## Methodology
1. Ensure tight contact between rods to minimize contact resistance.
2. Apply heat to one end of the setup.
3. Record temperatures at T1, T2, and T3 every 3 seconds using Arduino and data logger.
4. Wait for temperatures to stabilize to confirm steady-state.
5. Repeat the procedure for all three metal combinations.
6. Measure the physical dimensions (length and radius) of each rod.
7. Calculate experimental resistance using the temperature data and compare it with theoretical resistance based on Fourier’s law.

## Theory
Fourier’s law of heat conduction is used to determine theoretical resistance:

- R_theoretical = L / (k * A)  
- R_experimental = ΔT / Q  

Where L is the length of the rod, k is thermal conductivity, A is cross-sectional area, ΔT is temperature difference, and Q is the heat transfer rate.

Assumptions include one-dimensional steady-state conduction and perfect thermal contact.

## Results

| Setup   | R_exp (Ω) | R_theo (Ω) |
|---------|-----------|------------|
| Cu–Al   | 1.53      | 0.86       |
| Al–Fe   | 0.96      | 2.21       |
| Fe–Cu   | 0.96      | 1.70       |

Key observations:
- Experimental values show deviation from theoretical predictions.
- In the Cu–Al setup, experimental resistance was higher, likely due to contact resistance and heat losses.
- In Al–Fe and Fe–Cu, experimental resistance was lower than theoretical, possibly due to measurement uncertainties or unaccounted heat paths.

## Transient Analysis
- Cu–Al and Fe–Cu reached steady-state in approximately 25 minutes.
- Al–Fe took around 30 minutes, likely due to aluminum's higher specific heat and interface resistance.
- All setups showed a clear transient temperature rise followed by stabilization, consistent with simulated trends.

## Conclusion
- Experimental results generally follow the expected trend but differ quantitatively due to experimental limitations.
- Copper showed the lowest resistance, as expected due to its high thermal conductivity.
- Deviations arose from insulation inefficiency, imperfect contact, and external losses.

## Future Work
- Improve insulation to minimize heat loss.
- Incorporate contact resistance into theoretical modeling.
- Test more complex or non-metallic material combinations for broader application.

## Project Report
The complete project report with data and plots is available in the following file:  
[c9836806-6f43-4029-90d0-656cced58ae7.pdf](./c9836806-6f43-4029-90d0-656cced58ae7.pdf)

## License
This project was completed as part of the CHE212 course at IIT Kanpur and is intended for academic use.
