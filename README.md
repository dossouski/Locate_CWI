# Project Title: 
Automating data extraction from archives: Locating historical city-waste incineration sites in Durham, NC using city directories and Sanborn Fire Insurance maps

## Team Members
- Anselme Dossou
- Zilin Zhou

## Project Summary
Beneath the surface of bustling urban life lies a quiet accumulation of industrial and residential byproducts and hazardous materials that have long evaded public attention and regulatory oversight. Recent studies conducted in Durham NC, found lead contamination in the soil of several city parks, with some instances of contamination beginning 70 to 80 years ago. As waste incineration was a nationwide practice, locating old incineration sites is essential for understanding the full scope of urban environmental contamination. Historical records including city directories, newspapers and Sanborn maps are great resources that could be used to uncover the locations of those incinerators. The novelty of this work resides in the fact that it will develop a machine learning algorithm to search through pdf files. 

## Problem Statement / Objectives
The main objective is to develop a machine learning pipeline capable of automatically detect the keyword "incinerator" in city directories and Sanborn maps. 

## Datasets
Historic city directories and Sanborn maps: The library of Congress (LOC) holda a collection of these directories and historic maps that we could request online to train and test our algorithm on. 

## Python Packages Required
Specific packages
- libtesseract
- libleptonica
- tesserocr
Other packages (a lot more packages are needed to complete all the steps but we are just going to list a few here)
- numpy  
- pandas
- pickle
- time
- glob
- os
- sys

## Planned methods/approach
For this project we are planning to use similar methods as in Samuel Bell et al., 2020. The pipeline consists of the following discrete steps: grayscale thresholding, ad removal, margin cropping, cloumn chopping, line chopping, Optical Character Recognition, header identification, entry concatenation, text cleaning , address parsing, street matching and geocoding.  
## Expected outcomes
The project will yield a machine learning method able to read with high accuracy through pdf files. 
## Any other relevant information, images/tables, references, etc.
```{image} Durham_cd.jpg
:width: 600px
:align: center
```
## References
Bell S, Marlow T, Wombacher K, Hitt A, Parikh N, Zsom A, et al. (2020) Automated data extraction from historical city directories: The rise and fall of mid-century gas stations in Providence, RI. PLoS ONE 15(8): e0220219. https://doi.org/10.1371/journal.pone.0220219

Tollefson J, Frickel S, Restrepo MI (2021) Feature extraction and machine learning techniques for identifying historic urban environmental hazards: New methods to locate lost fossil fuel infrastructure in US cities. PLoS ONE 16(8): e0255507. https://doi.org/10.1371/journal.pone.0255507
