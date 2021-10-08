# EdgeFinder
EdgeFinder is a Mathematica Implementation of the Edge-to-Bump method for determining the position of an 'edge' in a distribution of data, relevant for kinematic distributions of variables like MT2. It was introduced in the paper

"Mixing It Up With MT2: Unbiased Mass Measurements at Hadron Colliders"
David Curtin, Dec 2011, arXiv:1112.1095 (Section 2).

It is particularly useful for fairly flat and smeared edges that are difficult to extract by other means.

Rather than performing a single particularly clever fit to extract the location of the edge or endpoint feature, the idea of the Edge-to-Bump method is to statistically analyze a distribution of fits over random subdomains of the data. Performing a huge number of simple fits goes a long way towards addressing issues of bias, unknown systematic error and choice of fit function, and supplies realistic error bars that include all sources of smearing for all the edges in a distribution.

This code is supplied for interested parties to quickly start playing with the basic ideas introduced in the paper. It's a proof-of-concept with much room for improvement, and one could think of many more sophisticated methods of analysing the distribution of fits than the simple one we used.

The code is quite slow in performing the 1000s of fits necessary to analyze a distribution (can take several hours). This can probably be improved significantly by compiling the code within Mathematica, but for serious applications one would want to implement the Edge-to-Bump method in a faster programming language, which would not be difficult

Feel free to contact me (david dot r dot curtin at gmail dot com) if you have any questions.

Downloads available in this repository:
* EdgeFinder 1.0 Mathematica Code (December 2011). This Mathematica Notebook is meant to be self-explanatory. It contains the EdgeFinder code, as well as several extensively commented examples that walk the user through the application of the code step-by-step. Hopefully this will be easier than a separate instruction manual, and allow the user to start applying the code to their own distributions very quickly. For a detailed explanation of the Edge-to-Bump method see Section 2 of the paper.
* Supplementary document to arXiv:1112.1095, containing all the edge-measurement plots from the two Monte Carlo studies in that paper. 

Citation

If you use this code in particular or the Edge-to-Bump method in general as part of your research, please cite arXiv:1112.1095.

