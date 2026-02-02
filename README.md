# Marine-clean-up-dives-remove-more-than-just-marine-debris
Payton, TG, Sims, RJ, Bulik, LT, &amp; Childress, MJ (2026). Marine clean-up dives remove more than just marine debris. Marine Pollution Bulletin

#Biomass Master Doc Workflow 
-contains excel workbook with tidy (parameter measurements), glance (goodness of fit metrics), and augment (model-level augmented predictions and diagnostics) outputs used to determine biomass models for each taxa with broom R package. 

#Biomass Medians Complete 
-contains medians, means, confidence intervals, sd, se, quartile, max, and min for taxa data used to create biomass models. 

#Equation Results Clean 
-contains weight measures for all taxa using median or biomass models for all taxa found on the 18 observed marine debris dives. 

#Biomass by ...
-taxa: gives basic statistic for biomass of taxa groups in grams and kilograms 
-material: gives basic statistics for biomass per material type in grams and kilograms 
-taxa_material: gives basic statistic for biomass per taxa group per material type in grams and kilograms 

#DAD Taxa Debris 
-Raw count data of taxa and litter material types by dive.

#mvabund ...
-multivariate statistics 
-univariate statistics

#PADI Mean Percent Per Year
-contains material type percent statistics for PADI AWARE reported dives from 2013-2023 after filtering for the Florida Keys, coral reef ecosystems, and dives containing at least one piece of debris.

#Sensitivy test plot
-Sensitivity of total biomass estimates to the minimum sample size required for applying length and width–weight relationships. Total biomass was calculated across a range of minimum sample-size cutoffs for applying length-weight and width-weight relationships (black line). For each cutoff, relationships were applied only when the taxon-specific sample size met or exceeded the cutoff and the equation could be evaluated successfully; all other observations used median mass values. The red horizontal line indicates total biomass estimated using median values only. Biomass estimates were highly sensitive to allowing relationships at very small sample sizes (n < ~7) but stabilized rapidly at higher cutoffs, indicating robustness of biomass estimates across a wide range of conservative thresholds.

#Spatial Variation
-Litter removal dive data were restricted to the Florida Keys reef tract (24.3–25.8°N, −82.0 to −80.0°W) to exclude implausible coordinates and ensure spatial comparability among sites. Dive locations were aggregated into spatial sites by rounding latitude and longitude to four decimal places (≈10–15 m), based on empirical assessment of coordinate variability for repeated visits to named sites. Each resulting spatial bin was treated as a unique site.
-Distance from shore was weakly but significantly correlated with debris counts (Spearman’s ρ = 0.18, p < 0.001; Fig. S1). However, variability in litter density (total counts) was high across all distances, and the magnitude of the relationship was small. Debris counts were weakly but significantly correlated with distance from shore (Spearman’s ρ = 0.176, p < 0.001), reflecting a small positive monotonic trend. However, variability in debris density was high across all distances, and the magnitude of the relationship was small, indicating that distance from shore explains only a limited portion of observed variation. 
-Relationship between distance from shore and (blue) total debris counts and (red) total litter weight. Smooth curves are generalized additive model (GAM) fits with 95% confidence intervals (shaded). Both debris counts and litter weight show weak non-linear trends with distance from shore, explaining only a small fraction of the observed variation (~6% for counts, ~11% for weight), indicating that distance is a minor driver of debris accumulation in the Florida Keys.

#Reef Visitation 
-To assess whether zero litter removals were associated with visitation frequency while accounting for repeated sampling and site-specific heterogeneity, we fitted a generalized linear mixed-effects model with a binomial error distribution and logit link function. The response variable was litter presence during a dive (binary: litter present vs. no litter removed). Visitation pressure was quantified as the total number of dives conducted at each site and entered as a log-transformed predictor. Year was included as a centered covariate to account for temporal trends. Site identity was included as a random intercept to account for repeated observations and persistent differences among sites. Models were fitted using maximum likelihood with Laplace approximation in the lme4 package in R.
-The probability of encountering litter during a dive decreased significantly with increasing visitation frequency (binomial GLMM; log-transformed visitation effect: β = −0.27 ± 0.10 SE, z = −2.82, p = 0.0049). This result indicates that more frequently visited sites were less likely to contain detectable litter, consistent with a visitation-driven removal effect. A significant negative temporal trend was also observed (β = −0.27 ± 0.04 SE, z = −6.00, p < 0.001), suggesting an overall decline in litter occurrence over the study period.
-Despite the significant effects of visitation and time, strong site-level heterogeneity remained. The random intercept for site identity exhibited substantial variance (σ² = 2.80), indicating large and persistent differences among sites in their baseline probability of litter occurrence. Intraclass correlation coefficients revealed that approximately 43–46% of the total variance in litter presence was attributable to site identity alone, after accounting for fixed effects. This demonstrates that nearly half of the observed zero inflation reflects inherent site-specific characteristics rather than visitation frequency or temporal trends.
-Spatial figure shows visited dive sites (points) along the Florida Keys color-coded by proportion of zero-litter dives where Yellow = almost always clean and Purple = almost never clean.

