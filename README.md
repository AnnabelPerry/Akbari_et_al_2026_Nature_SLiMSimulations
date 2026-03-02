# slim-selection-simulations
SLiM simulations described in sections "Test of selection on single variants", 
"Forward-in-time simulations of selection in the context of European history", 
and SUPPLEMENTARY INFORMATION SECTION 2 of Akbari et al. 2026, Nature

IMPORTANT The following file must be downloaded and placed in the `/inputs` 
sub-directory prior to running this code:
https://alkesgroup.broadinstitute.org/Eagle/downloads/tables/genetic_map_hg19_withX.txt.gz

### /scripts



## /inputs
Data files required for input into simulations

`non_overlapping_full_span_partition.tsv` Tab-separated file of UCSC Genome Browser (GENCODE_V47lift37 annotations), preprocessed according 
to the methods described in SUPPLEMENTARY INFORMATION SECTION 2 > SIMULATION OF EUROPEAN DEMOGRAPHIC HISTORY > Mutations
		
## /parameter_files
Files to be inputted into simulate.sh in order to run the 3 models described in the main text sections "Test of selection on single variants" 
and "Forward-in-time simulations of selection in the context of European history" as well as SUPPLEMENTARY INFORMATION SECTION 2. To use any of
these parameter files, you will need to adjust the directories named in the file to the actual directories for the indicated variable

`Model1Control_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 1 without directional selection
		
`Model1Experimental_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 1 with polygenic directional selection

`Model2.1Control_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 2.1 without directional selection

`Model2.1Experimental_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 2.1 with directional selection on a 
single standing variant

`Model2.2Control_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 2.2 without directional selection

`Model2.2Experimental_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 2.2 with directional selection on a 
single de novo variant

`Model3Control_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 3 without directional selection
		
`Model3Experimental_ParameterFile.txt` Parameter file which, when inputted to simulate.sh, runs Model 3 with polygenic directional selection

Parameter files required to reproduce the experiments described in subsection "Power analysis of GLMM and GLM and co-linearity" of SUPPLEMENTARY INFORMATION SECTION 2 are named in the below format:

Window100Kbp_S${PositiveCoeff}_ShiftGen_${ShiftGen}.txt

... where ${PositiveCoeff} is a placeholder for the --PositiveCoeff value while ${ShiftGen} is a placeholder for --ShiftGen value
