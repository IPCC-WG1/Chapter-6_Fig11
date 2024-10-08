TEMPORAL REGIONAL MEAN NET EFFECTIVE RADIATIVE FORCING DUE TO AEROSOLS
============

Figure number: Figure 6.11
From the IPCC Working Group I Contribution to the Sixth Assessment Report: Chapter 6

![Figure 6.11](/ar6_wg1_chap6_fig6_11_netERF_time_aer.png?raw=true)


Description:
------------
Time evolution of 5-year multi-model mean averages of the annual area-weighted mean regional net Effective Radiative Forcings (ERFs) due to aerosols for each of the 14 major regions in the Atlas, and global mean, using the models and model experiments as in Figure 6.10.

Author list:
------------
- Kuo, C: Lawrence Berkeley National Laboratory, USA; chaincy@berkeley.edu, chaincy.ipccwg1@gmail.com (lead only); githubid: chaincy-ipcc, githubid: chaincy-cal 


ESMValTool Branch:
------------------
- ESMValTool-AR6-OriginalCode-FinalFigures: [IPCC_AR6_WG1_Ch6](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/tree/IPCC_AR6_WG1_Ch6_ESMValTool)

Recipe & diagnostics:
---------------------
Recipe used:  
[recipes/ar6ch6/recipe_ckuo_ipcc_6_11_erf_histSST-piAer.yml](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/recipes/ar6ch6/recipe_ckuo_ipcc_6_11_erf_histSST-piAer.yml)

Recipe description:  
Time series of the upward top-of-the-atmosphere shortwave flux (rsut) and upward top-of-the-atmosphere flux (rlut) at each grid. The diagnostic scripts will calculate the annual mean effective radiative forcing (ERF) due to aerosols differencing shortwave and longwave fluxes between histSST-piAer and histSST AerChemMIP experiments.  

Diagnostics used:  
[diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py)  
ipcc_ar6wg1_fig6.11_erf_aer_time.py imports:   
* [diag_scripts/ar6ch6/cmapipcc.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/cmapipcc.py) 
 
Diagnostics description:
Script [diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py) calculates the gridded annual mean ERF of all models for IPCC AR6 WG1 Figure 6.11. 
The final Figure 6.11 is created from [ipcc_ar6wg1_Fig6.11.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig11/blob/main/ipcc_ar6wg1_Fig6.11.ipynb).


Expected data output path:
--------------------
This is the path of the time series data relative to the automatically generated ESMValTool output location:
- recipe_erf_histSST-piAer_Fig6.11_YYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf_time/LW_diff_timemap.nc   
- recipe_erf_histSST-piAer_Fig6.11_YYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf_time/SW_diff_timemap.nc   

Recipe generations tools: 
-------------------------  
N/A

Ancillary figures and datasets:
-------------------------------
The final Figure 6.11 is created by the following Jupyter notebook:  
[ipcc_ar6wg1_Fig6.11.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig11/blob/main/ipcc_ar6wg1_Fig6.11.ipynb).
The Jupyter notebook reads in netcdf output from [diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.11_erf_aer_time.py), which are output into the recipe path:  
- recipe_erf_histSST-piAer_Fig6.11_YYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf_time/LW_diff_timemap.nc   
- recipe_erf_histSST-piAer_Fig6.11_YYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf_time/SW_diff_timemap.nc   

Additional datasets:
--------------------
The AR6 WG1 Atlas reference regions are used to produce Figure 6.11.    
On the IPCC_AR6_WG1_Ch6_ESMValTool branch of ESMValTool-AR6-OriginalCode-FinalFigures:   
[diag_scripts/ar6ch6//data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.shp](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.shp)  
[diag_scripts/ar6ch6//data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.dbf](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.dbf)  
[diag_scripts/ar6ch6//data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.prj](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.prj)  
[diag_scripts/ar6ch6//data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.rda](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.rda)  
[diag_scripts/ar6ch6//data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.shx](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/data/regionmask/AR6_WGI_referenceRegions/AR6_WGI_referenceRegions.shx)  

What are their access permissions/Licenses?  
The license details can be found at https://github.com/IPCC-WG1/Atlas/blob/main/LICENSE.md    

Software description:
---------------------
- ESMValTool environment file: [IPCC_environments/ar6wg1_chap6_figs_conda_environment.yml](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/tree/main/IPCC_environments/ar6wg1_chap6_figs_conda_environment.yml)
- Other software used:  
A Jupyter notebook ([ipcc_ar6wg1_Fig6.11.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig11/blob/main/ipcc_ar6wg1_Fig6.11.ipynb)) is used to create Figure 6.11. See section "Ancillary figures and datasets" and "Additional datasets", above, for information.  

Hardware description:
---------------------
Machine used: Mistral  
 
When was this machine used?  
Last used July 2021 to produce figures from ESMValTool  
