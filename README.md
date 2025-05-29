**Space Weather Event Response Validation & Evaluation Hub (SWERVE Hub)** 

## Overview
This repository is part of the [ChronoStorm project](https://chronostorm.vercel.app), funded by the U.S. National Science Foundation (NSF) under grant [#2434136](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2434136). The project aims to collect and analyze perishable operational data from critical infrastructure sectors during significant space weather events, particularly during the solar maximum of Solar Cycle 25.

SWERVE Hub provides a centralized environment for validating and comparing space weather metrics for the May 2024 ("Gannon Storm"), including magnetic field variations, geoelectric field responses, and geomagnetically induced currents (GICs). This hub offers validated, cross-referenced data and tools for researchers and infrastructure stakeholders interested in space weather assessment.

## Project Background
In May 2024, Earth experienced a series of extreme space weather events, collectively referred to as the "Gannon Storm." These events included multiple Earth-directed coronal mass ejections (CMEs), triggering intense geomagnetic storms between May 10–12, 2024. 

The storm provided a rare opportunity to observe rapid fluctuations in Earth's magnetic field and to measure the resulting geoelectric fields and GICs, which pose risks to critical infrastructure, especially electrical power systems. The SWERVE Hub supports research into how different measurement and modeling approaches quantitatively compare in capturing these phenomena.

## Repository Contents
- **Data Files**: Magnetic field data, geoelectric field estimates, and GIC measurements from various sources during the May 2024 storm.
- **Analysis Scripts**: Code for preprocessing, analyzing, and visualizing the storm response across physical domains.
- **Documentation**: Descriptions of data sources, validation methodology, and results from comparative analyses.

## Goals
- Validate and compare a range of datasets and model outputs for storm-time metrics.
- Provide accessible, structured data for the research community.
- Support space weather infrastructure resilience efforts through better understanding of space weather impacts.

## Funding Acknowledgment
This work was supported by the U.S. National Science Foundation (NSF) under grant [#2434136](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2434136) as part of the ChronoStorm project. The research focuses on collecting and analyzing perishable operational data from critical infrastructure sectors during significant space weather events, aiming to enhance our understanding of infrastructure vulnerabilities and resilience. 

This grant is co-funded by the NSF GEO/AGS Space Weather Research program and the ENG/CMMI Humans, Disasters, and the Built Environment (HDBE) program.

## Data Acknowledgment
We kindly thank the Tennessee Valley Authority (TVA) for providing data from their internal GIC estimation model, reflecting the realistic circuit configuration over the May 10-12th 2024 period. Without TVA's support, and this perishable data, we would struggle to compare predictive metrics to this more reliable baseline. 

## Contributors 
- Lucy Wilkerson - Graduate Research Assistant (lwilker [ at ] gmu [ dot ] edu) 
- Bob Weigel - Senior Personnel (rweigel [ at ] gmu [ dot ] edu)
- Dean Thomas - Research Fellow (dthomas6 [ at ] gmu [ dot ] edu) 
- Edward Oughton - Primary Investigator (eoughton [ at ] gmu [ dot ] edu)

## License
This repository is licensed under the MIT License. See `LICENSE` for details.

# Maps w GIC and magnetometer sites
![](_map/map.png)

![](_map/map_zoom_tva.png)

# Transmission line analysis

![](_results/transmission_map.png)

![](_results/transmission_std_map.png)

![](_results/trans_lines_TVA.png)

![](_results/trans_lines_count.png)

![](_results/trans_lines_length.png)

# Data plots for paper

![](_processed/_tva/gic_tva.png)

![](_processed/_nerc/gic_nerc.png)

![](_imf/imf_mage.png)

![](_imf/imf_all.png)

# TVA GIC vs GIC modeled (TVA and GMU)

![](_processed/bullrun/GIC_compare_timeseries.png)

![](_processed/bullrun/GIC_compare_correlation.png)

![](_processed/montgomery/GIC_compare_timeseries.png)

![](_processed/montgomery/GIC_compare_correlation.png)

![](_processed/union/GIC_compare_timeseries.png)

![](_processed/union/GIC_compare_correlation.png)

![](_processed/widowscreek/GIC_compare_timeseries.png)

![](_processed/widowscreek/GIC_compare_correlation.png)

for all GIC timeseries comparisons, see ![GIC markdown](GIC_compare_timeseries.md)

for just TVA GIC timeseries comparisons, see ![TVA GIC markdown](GIC_compare_timeseries_TVA.md)

for just GMU GIC timeseries comparisons, see ![GMU GIC markdown](GIC_compare_timeseries_GMU.md)

# TVA B vs MAGE/SWMF modeled

![](_processed/bullrun/B_compare_timeseries.png)

![](_processed/bullrun/B_compare_correlation.png)

![](_processed/union/B_compare_timeseries.png)

![](_processed/union/B_compare_correlation.png)

for all B timeseries comparisons, see ![B markdown](B_compare_timeseries.md)

# GIC Time Series Comparisons for site pairs

![](_results/pairs/bullrun_montgomery.png)

![](_results/pairs/bullrun_union.png)

![](_results/pairs/bullrun_widowscreek.png)

![](_results/pairs/montgomery_union.png)

![](_results/pairs/montgomery_widowscreek.png)

![](_results/pairs/union_widowscreek.png)

similar figures for all site pairs (2024-AGU-data/_results/pairs/site1_site2.png)
or see ![pairs markdown](GIC_compare_pairs.md)

# Cross Correlation of Site Pairs

![](_results/pairs/xcorr_scatter.png)

see ![here](GIC_compare_pairs.md) for cross correlation analysis of each pair

# GIC CC-Distance Map Comparisons

![](_results/cc_vs_dist_map.png)

![](_processed/bullrun/cc_vs_dist_map.png)
similar figures for 55 more sites (2024-AGU-data/_processed/sitename/cc_vs_dist_map.png)

# GIC CC-Distance Scatter Comparisons

![](_results/cc_vs_dist_scatter.png)

![](_results/cc_vs_dist_grid_scatter.png)

![](_processed/bullrun/cc_vs_dist_scatter.png)
similar figures for 55 more sites (2024-AGU-data/_processed/sitename/cc_vs_dist_scatter.png)

# GIC CC-StDev Scatter Comparisons

![](_results/cc_vs_std_scatter.png)

![](_results/cc_vs_std_grid_scatter.png)

![](_processed/bullrun/cc_vs_std_scatter.png)
similar figures for 55 more sites (2024-AGU-data/_processed/sitename/cc_vs_std_scatter.png)

# GIC CC-Beta Scatter Comparisons

![](_results/cc_vs_beta_scatter.png)

![](_results/cc_vs_beta_grid_scatter.png)

![](_processed/bullrun/cc_vs_beta_scatter.png)
similar figures for 55 more sites (2024-AGU-data/_processed/sitename/cc_vs_beta_scatter.png)

# GIC CC-Line Voltage Scatter Comparisons

![](_results/cc_vs_volt_scatter.png)

![](_results/cc_vs_volt_grid_scatter.png)

# GIC CC-Latitude Comparisons

![](_results/cc_vs_lat_scatter.png)

![](_results/cc_vs_lat_grid_scatter.png)

# GIC CC-Dist Scatter Comparison w colors

![](_results/cc_vs_dist_vs_beta_scatter.png)

![](_results/cc_vs_dist_vs_volt_scatter.png)

![](_results/cc_vs_dist_vs_lat_scatter.png)

# GIC StDev Scatter Plots

![](_results/std_vs_beta_scatter.png)

![](_results/std_vs_lat_scatter.png)

# Regression Analysis
## Correlation coefficient between GIC site pairs
![](_results/scatter_fit_dist(km)_cc.png)

![](_results/scatter_fit_beta_diff_cc.png)

![](_results/scatter_fit_lat_diff_cc.png)

![](_results/scatter_fit_all_cc.png)

![](_results/scatter_fit_cross_cc.png)

## Standard deviation of GIC at each site
![](_results/scatter_fit_interpolated_beta_std.png)

![](_results/scatter_fit_geo_lat_std.png)

![](_results/scatter_fit_all_std.png)

![](_results/scatter_fit_cross_std.png)

## Peak GIC at each site
![](_results/scatter_fit_interpolated_beta_gic_max.png)

![](_results/scatter_fit_geo_lat_gic_max.png)

![](_results/scatter_fit_all_gic_max.png)

![](_results/scatter_fit_cross_gic_max.png)


