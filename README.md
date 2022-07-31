# OdorMappingData
Glomerular response datasets. 

Credits: S. Burton (data collection, analysis), A. Brown (analysis), M. Wachowiak (analysis), T. Rust (software).

Parent manuscript: 
Mapping odorant sensitivities reveals a sparse but structured representation of olfactory chemical space by sensory input to the mouse olfactory bulb.

Shawn D. Burton1, Audrey Brown1, Thomas P. Eiting1, Isaac A. Youngstrom1, Thomas C. Rust1, Michael Schmuker2, Matt Wachowiak1

https://elifesciences.org/articles/80470

See Materials and Methods of above manuscript for details of data collection and pre-processing pipeline. Description of .mat file is below:

‘odormappingdata_simple_05_22.mat’ file. 
Variables:
	'allrespmatrices_dF': Structure array consists of odorant response matrices and ROI positions for each OB. Variables are indexed in the following order: (1) omp111L, (2) omp111R, (3) omp112L, (4) omp112R, (5) omp113L, (6) omp113R, (7) omp114L, (8) omp114R. All odorants are in the same order for all response matrices (see ‘odornameslist’ variable).
ROI positions indicate centroid of each ROI, after visual registration by aligning the midline and caudal sinus. Units are microns, reference (zero) is midline (for ‘Xpos’) and caudal sinus (for ‘Ypos’). Note that the Xposition for ROIs from the left OB is negative relative to midline.
	'allconcs_prep': Calculated final delivered concentration of each odorant, indexed in the same order as response matrices and odornames list, for each mouse, in mols/L. Note that concentrations estimated from vapor pressure, calibrated air dilution, and liquid dilution, assuming ideal behavior. 
	'odornameslist': List of all 185 odorants (plus two vehicle controls), indexed in same order as odors in response spectrum matrices.



