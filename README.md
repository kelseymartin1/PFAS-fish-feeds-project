PFAS-fish-feeds-project

This project seeks to explore the levels of per- and polyfluoroalkyl substances (PFAS) that are present in commercially available fish feeds. 

The questions we seek to answer are:
1. At what levels are PFAS present in fish feeds?
2. Do feeds higher in fish meal (fm) have higher PFAS content than those with plant protein (pp), animal protein (ap), and soybean meal (sm)?
3. Do feeds with a higher protein percentage (protein_per) have higher PFAS content?
4. Are there significant differences in PFAS content between manufacturers (mfr)?

Data were collected by analyzing each feed using liquid chromatography tandem mass spectrometry in the Fall of 2022. 

I will be looking at 4 compounds. These compounds are PFOS, PFNA, PFDA, and PFUnA. 

The .csv file is titled 'feed_pfas.csv'. It is structured into separate columns for each variable (protein_per, protein_source, mfr) and each compounds (PFOS, PFNA, PFDA, PFUnA).

The data was read into R.

Counts for both categorical variables (protein_source and mfr) were calculated to determine sample size. Inadequate sample size (less than 3) resulted in that group being omitted.

Animal protein (ap) and plant protein (pp), as well as manufacturers B and E were subsetted out of the data. The new dataset is now called subset_feeds.

Categorical variables were then factored so as to carry out multiple linear regression analyses.

Mixed effects models were conducted to investigate the significance between PFAS concentrations and protein content, protein source, and manufacturer.
