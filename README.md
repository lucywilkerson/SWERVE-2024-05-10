# Overview
This repository is part of the [ChronoStorm project](https://chronostorm.vercel.app), funded by the U.S. National Science Foundation (NSF) under grant [#2434136](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2434136).

The source code and project details are available in the [SWERVE](https://github.com/lucywilkerson/SWERVE) repository.

**Paper citation**

Lucy Wilkerson, Robert S Weigel, Dean Thomas, et al. GIC-Related Observations During the May 2024 Geomagnetic Storm in the United States. _ESS Open Archive_. October 16, 2025. doi: https://doi.org/10.22541/essoar.176062871.15246663/v1

# Data Organization

All unprocessed data can be found in data_original. Measured GIC and B from NERC are in [nerc](data_original/nerc); measured and calculated GIC and measured B from TVA are in [tva](data_original/tva); calculated GIC from the Reference model are in [gmu](data_original/gmu); calculated B from MAGE are in [mage](data_original/mage); calculated B from SWMF are in [swmf](data_original/swmf); calculated B from OpenGGCM are in [openggcm](data_original/openggcm); solar wind inputs used for the MAGE and SWMF/OpenGGCM runs are in [bcwind.h5](data_original/imf_data/bcwind.h5) and [Dean_IMF.txt](data_original/imf_data/Dean_IMF.txt), respectively. 

Processed data are organized by site in [data_processed/sites](data_processed/sites), with each site having its own _all.pkl file containing the processed data.

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

![](data_processed/summary/_tva/gic_tva.png)

![](data_processed/summary/_nerc/gic_nerc.png)

![](data_processed/summary/_db/db_all.png)

![](data_processed/summary/_imf/imf_hapi.png)

![](data_processed/summary/_imf/imf_all.png)

# TVA GIC vs GIC modeled (TVA and GMU)

![](data_processed/sites/bullrun/figures/compare/GIC_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/bullrun/figures/compare/GIC_calculated_all_vs_measured_scatter.png)

![](data_processed/sites/montgomery/figures/compare/GIC_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/montgomery/figures/compare/GIC_calculated_all_vs_measured_scatter.png)

![](data_processed/sites/union/figures/compare/GIC_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/union/figures/compare/GIC_calculated_all_vs_measured_scatter.png)

![](data_processed/sites/widowscreek/figures/compare/GIC_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/widowscreek/figures/compare/GIC_calculated_all_vs_measured_scatter.png)

for all GIC timeseries comparisons, see ![GIC markdown](GIC_compare_timeseries.md)

for just TVA GIC timeseries comparisons, see ![TVA GIC markdown](GIC_compare_timeseries_TVA.md)

for just GMU GIC timeseries comparisons, see ![GMU GIC markdown](GIC_compare_timeseries_GMU.md)

# TVA B vs MAGE/SWMF/OpenGGCM modeled

![](data_processed/sites/bullrun/figures/compare/B_HBzByBx_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/bullrun/figures/compare/B_HBzByBx_calculated_all_vs_measured_scatter.png)

![](data_processed/sites/union/figures/compare/B_HBzByBx_calculated_all_vs_measured_timeseries.png)

![](data_processed/sites/union/figures/compare/B_HBzByBx_calculated_all_vs_measured_scatter.png)

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

![](_results/plot_scatter/cc_vs_dist_map.png)

# CC-Distance Scatter Comparisons

## GIC

![](_results/plot_scatter/cc_vs_dist_scatter.png)

![](_results/plot_scatter/cc_vs_dist_grid_scatter.png)

## B_H

![](_results/plot_scatter/cc_vs_dist_scatter_B.png)

# CC-StDev Scatter Comparisons

## GIC

![](_results/plot_scatter/cc_vs_std_scatter.png)

![](_results/plot_scatter/cc_vs_std_grid_scatter.png)

## B_H

![](_results/plot_scatter/cc_vs_std_scatter_B.png)

# CC-Beta Scatter Comparisons

## GIC

![](_results/plot_scatter/cc_vs_beta_scatter.png) 

![](_results/plot_scatter/cc_vs_logbeta_scatter.png)

![](_results/plot_scatter/cc_vs_beta_grid_scatter.png)

## B_H

![](_results/plot_scatter/cc_vs_logbeta_scatter_B.png)

![](_results/plot_scatter/cc_vs_beta_scatter_B.png)

# CC-Line Voltage Scatter Comparisons

## GIC

![](_results/plot_scatter/cc_vs_volt_scatter.png)

![](_results/plot_scatter/cc_vs_volt_grid_scatter.png)

## B_H

![](_results/plot_scatter/cc_vs_volt_scatter_B.png)

# CC-Latitude Comparisons

## GIC

![](_results/plot_scatter/cc_vs_lat_scatter.png)

![](_results/plot_scatter/cc_vs_lat_grid_scatter.png)

## B_H

![](_results/plot_scatter/cc_vs_lat_scatter_B.png)

# GIC CC-Dist Scatter Comparison w colors

![](_results/plot_scatter/cc_vs_dist_vs_beta_scatter.png)

![](_results/plot_scatter/cc_vs_dist_vs_volt_scatter.png)

![](_results/plot_scatter/cc_vs_dist_vs_lat_scatter.png)

# GIC StDev Scatter Plots

![](_results/plot_scatter/std_vs_beta_scatter.png)

![](_results/plot_scatter/std_vs_lat_scatter.png)

# Regression Analysis
see [linear_regression.md](linear_regression.md) for more detailed analysis
## Correlation coefficient between GIC site pairs
![](_results/regression/scatter_fit_dist(km)_cc.png)

![](_results/regression/scatter_fit_beta_diff_cc.png)

![](_results/regression/scatter_fit_lat_diff_cc.png)

![](_results/regression/scatter_fit_all_cc.png)

![](_results/regression/scatter_fit_cross_cc.png)

## Standard deviation of GIC at each site
![](_results/regression/line_fit_interpolated_beta_std.png)

![](_results/regression/scatter_fit_interpolated_beta_std.png)

![](_results/regression/line_fit_log_beta_std.png)

![](_results/regression/scatter_fit_log_beta_std.png)

![](_results/regression/line_fit_geo_lat_std.png)

![](_results/regression/scatter_fit_geo_lat_std.png)

![](_results/regression/line_fit_alpha_std.png)

![](_results/regression/scatter_fit_alpha_std.png)

![](_results/regression/scatter_fit_all_std.png)

![](_results/regression/scatter_fit_cross_std.png)

Table with results: ![fit_table_std.md](_results/regression/fit_table_std.md)

## Peak GIC at each site
![](_results/regression/line_fit_alpha_interpolated_beta_gic_max_manual_error.png)

![](_results/regression/scatter_fit_alpha_interpolated_beta_gic_max_manual_error.png)

![](_results/regression/line_fit_interpolated_beta_gic_max_manual_error.png)

![](_results/regression/scatter_fit_interpolated_beta_gic_max_manual_error.png)

![](_results/regression/line_fit_alpha_gic_max_manual_error.png)

![](_results/regression/scatter_fit_alpha_gic_max_manual_error.png)

Table with results: ![fit_table_gic_max_manual_error.md](_results/regression/fit_table_gic_max_manual_error.md)

Older plots:

![](_results/regression/line_fit_log_beta_gic_max.png)

![](_results/regression/scatter_fit_log_beta_gic_max.png)

![](_results/regression/line_fit_geo_lat_gic_max.png)

![](_results/regression/scatter_fit_geo_lat_gic_max.png)

![](_results/regression/scatter_fit_all_gic_max.png)

![](_results/regression/scatter_fit_cross_gic_max.png)
