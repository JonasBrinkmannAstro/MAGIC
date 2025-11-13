M.A.X. - MUSE Absorption eXtractor


MAX is an end-to-end spectral analysis pipeline designed to extract, model and interpret absorption lines in background galaxy spectra emprinted by foreground Galaxies for MUSE data cubes.
Thank you for downloading this script. I hope it is useful for your research.
Acknowledgement of this work is appreciated.

This workflow is designed to run in a Jupyter Notebook environment.
The main script is divided into multiple substeps. Interim results (such as CSV files and summed FITS files) are stored and later loaded from the interim_processing folder.
All scripts are set up so that an example run can be conducted simply by executing each code cell in order.

The data cube should be placed in the same folder as the script.
The provided data cube is publicly available under:
👉 https://amused.univ-lyon1.fr/project/megaflow/download
one of the dowloaded data cubes should be: 
J0014m0028_dr2_zap_wpsf1_qsosub.corrEBV and should be placed in the same folder as the script and the naming kept intact.

Credit: Bouché et al. (2024). If you use this cube, please also acknowledge their work.

Most adjustable parameters are grouped and clearly marked within each script.

Required packages:
	-numpy
	-pandas
	-scipy
	-matplotlib
	-astropy
	-scikit-learn
	-scikit-image
	-emcee
	-corner

The steps of the data processing performed by each subscript correspond to the stages shown in Figure 3.1 of the thesis.

I hope you find this usefull for your specific work — happy coding!      
⠀⠀⠀⠀⠀ ⠀⠀⠀    ⠀⢠⣿⣶⣄⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀  
⠀⠀⠀⠀⠀⠀⠀⢀⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⣶⣦⣄⣀⡀⣠⣾⡇⠀⠀⠀⠀  
⠀⠀⠀⠀⠀⠀⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀⠀⠀⠀  
⠀⠀⠀⠀⠀⢀⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠿⠿⢿⣿⣿⡇⠀⠀⠀⠀  
⠀⣶⣿⣦⣜⣿⣿⣿⡟⠻⣿⣿⣿⣿⣿⣿⣿⡿⢿⡏⣴⣺⣦⣙⣿⣷⣄⠀⠀⠀  
⠀⣯⡇⣻⣿⣿⣿⣿⣷⣾⣿⣬⣥⣭⣽⣿⣿⣧⣼⡇⣯⣇⣹⣿⣿⣿⣿⣧⠀⠀  
⠀⠹⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠸⣿⣿⣿⣿⣿⣿⣿⣷ 
