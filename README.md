PFAS-fish-feeds-project

This project seeks to explore the levels of per- and polyfluoroalkyl substances (PFAS) that are present in commercially available fish feeds. 

The questions we seek to answer are:
1. At what levels are PFAS present in fish feeds?
2. Do feeds higher in fish meal (fm) have higher PFAS content than those with plant protein (pp), animal protein (ap), and soybean meal (sm)?
3. Do feeds with a higher protein percentage (protein_per) have higher PFAS content?
4. Are there significant differences in PFAS content between manufacturers (mfr)?

Data were collected by analyzing each feed using liquid chromatography tandem mass spectrometry in the Fall of 2022. 

The final .Rmd file is titled "mixed_effects_models.Rmd"

A pdf of the analysis is included.

The data folder include the .csv file used for the analysis, as well as the metadata.

The Figures folder includes all figures created in the analysis.

I will be looking at 4 compounds. These compounds are PFOS, PFNA, PFDA, and PFUnA. 

The .csv file is titled 'feeds_restructured.csv'.

The data was read into R.

Counts for both categorical variables (protein_source and mfr) were calculated to determine sample size. Inadequate sample size (less than 3) resulted in that group being omitted.

Animal protein (ap) and plant protein (pp), as well as manufacturers B and E were subsetted out of the data. The new dataset is now called subset_feeds.

Categorical variables were then factored.

Mixed effects models were conducted to investigate the significance between PFAS concentrations and protein content, protein source, and manufacturer.
