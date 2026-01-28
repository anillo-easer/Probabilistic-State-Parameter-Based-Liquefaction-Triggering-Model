# Probabilistic-State-Parameter-Based-Liquefaction-Triggering-Model

Probabilistic State Parameter-Based Liquefaction Triggering Model, software, data, and documentation

This repository comprises the information used in the article: "Probabilistic State Parameter-Based Liquefaction Triggering Model." by Pedro Reyes, Gonzalo Montalva, Vicente San Martín, and Robb Moss submitted to the Journal of Geotechnical and Geoenvironmental Engineering (ASCE).

Liquefaction Triggering Model (CPT_to_PL.R)
This package reproduces the CPT-based probabilistic workflow used in our liquefaction triggering study. Resistance CRR(ψ) is combined with Monte Carlo propagation of the CPT-derived state parameter ψ (Plewes-type) and probabilistic seismic demand CSR to compute PL versus depth. 

How to use it:
1.	Set the working directory to the folder that contains: CPT.xlsx, CRR_model.RData, CSR_model.RData, and PSI_uncertainty.RData.
Example: setwd("C:/Users/X/Downloads/CPT_to_PL")
2.	Edit the following inputs: GWT (m), amax, Mw, n_mc, and (optional) K0_user, Mtc_user, a_ratio_user.
3.	Run the script.

Output: CPT_profile_panels.png will be saved in the same folder, showing q_c (MPa), R_f (%), I_(c,RW), ψ, CRR(ψ), P_L versus depth.

Laboratory database (Lab_Tx_Database_2026.xlsx)
The file contains the database comprising laboratory cyclic and monotonic triaxial test results and associated metadata used to calibrate the model presented in the manuscript.
The database includes: the summary table reported in the article with the parameters used in the study; CSL (Critical State Line) and LRC (liquefaction resistance curves) data used for calibration; one worksheet per material, containing the individual test results for that material.

Acknowledgment
This study was supported by Chile’s National Agency for Research and Development (ANID) through the BECAS/MAGÍSTER NACIONAL program (Grant 22240930) and the Anillo EASER Evolution Assessment of Seismic Risk (Grant ACT240044). The authors also thank the Geotechnical Group at the Universidad de Concepción, Chile.
