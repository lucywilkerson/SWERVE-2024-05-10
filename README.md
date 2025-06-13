# Overview
This repository is part of the [ChronoStorm project](https://chronostorm.vercel.app), funded by the U.S. National Science Foundation (NSF) under grant [#2434136](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2434136).

The source code and project details are available in the [SWERVE](https://github.com/lucywilkerson/SWERVE) repository.

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

![](_processed/_db/db_all.png)

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

![](_results/cc_vs_logbeta_scatter.png)

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
see [linear_regression.md](linear_regression.md) for more detailed analysis
## Correlation coefficient between GIC site pairs
![](_results/scatter_fit_dist(km)_cc.png)

![](_results/scatter_fit_beta_diff_cc.png)

![](_results/scatter_fit_lat_diff_cc.png)

![](_results/scatter_fit_all_cc.png)

![](_results/scatter_fit_cross_cc.png)

## Standard deviation of GIC at each site
![](_results/line_fit_interpolated_beta_std.png)

![](_results/scatter_fit_interpolated_beta_std.png)

![](_results/line_fit_log_beta_std.png)

![](_results/scatter_fit_log_beta_std.png)

![](_results/line_fit_geo_lat_std.png)

![](_results/scatter_fit_geo_lat_std.png)

![](_results/scatter_fit_all_std.png)

![](_results/scatter_fit_cross_std.png)

Table with results: ![fit_table_std.md](_results/fit_table_std.md)

## Peak GIC at each site
![](_results/line_fit_interpolated_beta_gic_max.png)

![](_results/scatter_fit_interpolated_beta_gic_max.png)

![](_results/line_fit_log_beta_gic_max.png)

![](_results/scatter_fit_log_beta_gic_max.png)

![](_results/line_fit_geo_lat_gic_max.png)

![](_results/scatter_fit_geo_lat_gic_max.png)

![](_results/scatter_fit_all_gic_max.png)

![](_results/scatter_fit_cross_gic_max.png)

Table with results: ![fit_table_gic_max.md](_results/fit_table_gic_max.md)
