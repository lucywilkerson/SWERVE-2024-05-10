
**Introduction**

The files in this directory contain Biot-Savart analysis determining the delta B changes in the magnetic field on Earth due to magnetospheric, gap region, and ionospheric contributions.  The results are based on an SWMF simulation of the Gannon storm, and uses python code at:

https://github.com/dthoma6/deltaB/tree/GIC

The total change in magnetic field on Earth (delta B) is the sum of the magnetospheric, gap region, and ionospheric contributions.  The data does not include the baseline magnetic field due to the Earth’s dipole or Telleric contributions.

**Filenames**

In this directory, file names are of the form:

dB_site.pkl 
dB_site.csv

where site is one of the following:

| Site | Latitude | Longitude |
|----|----|----|
| 50100 | 30.4 |89.6 |
| 50127 | 37.1 | 119.7 |
| 50112 | 48.3 | 117.1 |
| 50131 | 37.8 | 84.7 |
| 50132 | 38 | 84.8 |
| 50103 | 33.3 | 89.2 |
| 50104 | 36 | 84.1 |
| 50109 | 35.6 | 84.7 |
| 50115 | 41.3 | 90.5 |
| 50116 | 37.2 | 86.9 |
| 50117 | 36.1 | 81 |
| 50118 | 39.4 | 87.4 |
| 50119 | 35 | 85.3 |
| 50120 | 34.3 | 88.8 |
| 50122 | 35.6 | 89.3 |
| Montgomery | 36.5949 | 87.2533 |
| Widows Creek | 34.8859 | 85.7554 |
| Bull Run | 36.0193 | 84.1575 |
| Union | 34.378 | 88.8578 |

**Breakdown of magnetospheric currents**

In the analysis, the magnetospheric current densities are broken down into currents parallel and perpendicular to the magnetosphere’s local magnetic field.   And the perpendicular component is futher decomposed into components parallel to azimuth and a residual term.  These components are used to determine the magnetic filed on Earth due to various magnetospheric currents.

For more details, see Section 3 of  https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024JA032556 

**Variables**

Each file contains the changes in the magnetic field (delta B) at the latitude-longitude specified.  The pickle files (.pkl) and the CSV files (.csv) contain the same data.  The only difference is
missing data in the pickle files are labeled ‘nan’, while in the CSV files, they are blank.  The pickle dataframe has a Timestamp index, which is equivalent to the Datetime column. 

The following data are provided:
* Timestamp - Time associated with measurements in YYYY-MM-DD HH:MM:SS.  In the pickle files, this is the dataframe index. <br>
* Bn_msph, Be_msph, Bd_msph -  North, East, and Down components of the change in the magnetic field due to magnetospheric currents  <br>
* Bparan_msph, Bparae_msph, Bparad_msph - North, East, and Down components of the change in the magnetic field due to magnetospheric currents parallel to the local magnetospheric magnetic field  <br>
* Bperpn_msph, Bperpe_msph, Bperpd_msph - North, East, and Down components of the change in the magnetic field due to magnetospheric currents perpendicular to the local magnetospheric magnetic field  <br>
* Bperpphin_msph, Bperpphie_msph, Bperpphid_msph - North, East, and Down components of the change in the magnetic field due to magnetospheric currents perpendicular to the local magnetospheric magnetic field  and in the azimuthal direction   <br>
* Bperpresn_msph, Bperprese_msph, Bperpresd_msph - North, East, and Down components of the change in the magnetic field due to residual component of magnetospheric currents   <br>
* Bx_msph, By_msph, Bz_msph - X,Y,Z components in SM coordinates of the change in the magnetic field due to magnetospheric currents  <br>
* Bn_gap, Be_gap, Bd_gap - North, East, and Down components of the change in the magnetic field due to gap region field-aligned currents  <br>
* Bx_gap, By_gap, Bz_gap - X,Y,Z components in SM coordinates of the change in the magnetic field due to gap region field-aligned currents  <br>
* Bnp_iono, Bep_iono, Bdp_iono -  North, East, and Down components of the change in the magnetic field due to Pedersen ionospheric currents  <br>
* Bxp_iono, Byp_iono, Bzp_iono - X,Y,Z components in SM coordinates of the change in the magnetic field due to Pedersen ionospheric currents  <br>
* Bnh_iono, Beh_iono, Bdh_iono - North, East, and Down components of the change in the magnetic field due to Hall ionospheric currents  <br>
* Bxh_iono, Byh_iono, Bzh_iono -  X,Y,Z components in SM coordinatesof the change in the magnetic field due to Hall ionospheric currents  <br>
* Datetime - Time associated with measurements in YYYY-MM-DD HH:MM:SS.   In the pickle files, this is a datetime data type.  <br>
