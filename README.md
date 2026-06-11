# Relativistic Particle Interactions: Statistical Modeling of Compton Scattering
## Author: ShiTeng Mei | Project Date: Fall 2024 

# Project Overview
This project, conducted as part of the advanced physics lab curriculum at Stony Brook University (December 2024), investigates the foundational principles of the Compton effect to experimentally verify the relativistic parameters of subatomic particles. Using an experimental Compton scattering apparatus to measure the energy and count rates of scattered gamma rays within specific solid angles, the project successfully achieves three primary data objectives:
* Relativistic Energy Verification: Measured the rest energy of an electron to be approximately $0.570 \pm 0.016 \text{ MeV}$ and the energy of an incident gamma ray to be approximately $0.705 \pm 0.017 \text{ MeV}$.
* Cross-Section Model Evaluation: Constructed an experimental graph of the differential cross-section across multiple angles, comparing the data against classical Thomson scattering and quantum Klein-Nishina (K-N) formulas. Minimum chi-square calculations yielded $\chi^2 = 70.16$ for the K-N model and $\chi^2 = 1340.37$ for the Thomson model, quantitatively proving that the quantum mechanical K-N model provides a superior approximation for relativistic observed results.
* Material Yield Quantification: Determined the total free electron counts in small aluminum (Al) and copper (Cu) scatterers, evaluating their respective yield ratios at scattering coordinates of 25° (obtaining 0.86) and 45° (obtaining 0.64).  

# Libraries/Tools: 
* Multi-Channel Analyzer (MCA) software, Oscilloscope digitization
* Mathematical Models: Gaussian Distribution Fitting (python), Linear Regression (spreadsheet), Minimum Chi-Square ($\chi^2$) Analysis, and Data Layout & Tracking uses Spreadsheet software (Excel).

# Data Processing WorkflowSignal Acquisition: 
* Captured raw electrical pulse counts from gamma-ray interactions with Aluminum and Copper scatterers.
* Background Correction: Mathematically subtracted environmental radiation noise to isolate significant events.
* Calibration: Developed a linear calibration model to map MCA channel numbers to specific energy values in keV.
* Gaussian Modeling: Applied Gaussian distributions to photopeaks to identify the "true" energy center and account for detector resolution.
* Attenuation Analysis: Calculated material-specific attenuation coefficients to verify the density-dependent nature of particle interaction.

# Key Findings
* Relativistic Parameter Verification: Experimentally determined the electron rest mass energy to be $0.570 \pm 0.016 \text{ MeV}$ (an $11.5\%$ variation from theoretical values) and the incident gamma-ray energy from the $^{137}\text{Cs}$ source to be $0.705 \pm 0.017 \text{ MeV}$ ($6.5\%$ variation from theory).
* Mathematical Model Optimization: Quantified the validity of quantum vs. classical scattering models using least-squares regression across twelve angular points ($18^{\circ}$ to $110^{\circ}$). The quantum Klein-Nishina model yielded a minimum chi-square ($\chi^2_{\text{min}}$) of $70.16$, comprehensively outperforming the classical Thomson model’s $\chi^2_{\text{min}}$ of $1340.37$ and confirming quantum field theory approximations.
* System Calibration Accuracy: Established a linear relationship mapping Multi-Channel Analyzer (MCA) data channels to physical energy spectrum scales: $E = (0.0031 \pm 0.0001)\text{channel} + (-0.0633 \pm 0.0210)$, backed by a Gaussian curve-fitting linear regression model scoring a reliable $P\text{-value} \approx 2\%$ at a $1\%$ significance level.
* Volumetric Mass Attenuation: Determined the effective square thickness ($d_{\text{experimental}}$) of the large Aluminum scatterer to be $4.98 \pm 0.34\text{ cm}$ via beam attenuation tracking, showing an accurate $2\%$ deviation from the physical geometric average of $4.99\text{ cm}$.
* Material Free-Electron Discrepancy: Evaluated target scatterer material yields (Copper over Aluminum), obtaining ratio values of $0.86$ at $25^{\circ}$ and $0.64$ at $45^{\circ}$ (averaging $0.75$). This data exposed an experimental boundary where atomic electron binding energies lower actual free electron yields relative to theoretical total electron capacities ($1.66 \times 10^{26}$ for Cu vs. $4.26 \times 10^{25}$ for Al).  

# Repository Structure
* Python source files (.py or .ipynb) written for data cleanup, modeling, and plotting:
* * [Compton scattering three curves notebook](compton_scattering_three_curves.ipynb)
  * [curve_fitting_of_total_absorption_efficiency](curve_fitting_of_total_absorption_efficiency.ipynb)
  * [gaussian_fit_reading_data_version1](gaussian_fit_reading_data_version1.ipynb)
  * [integral_under_the_entire_fitting_curve](integral_under_the_entire_fitting_curve.ipynb)
    
# The final report
* * [Compton scattering](Final version compton scattering.pdf)




