# Cliff-Lorimer-Analysis
This project aims to perform Cliff-Lorimer analysis on thin samples examined by TEM-EDXS in order to elementally characterize the sample.

When a sample is exposed to an electron beam (as in Transmission Electron Microscopy [TEM]) the sample will emit characteristic X-rays.
Analyzing these X-rays to quantify the elemental makeup of this sample is called Energy Dispersive X-ray Spectroscpy (EDXS).

Elemental quantification of thick samples requires corrections for X-ray absorption, X-ray flourescence, and Z (atomic weight) factors, called ZAF corrections.
Thin samples (< 100 nm) can be simplified by assuming the absorption and flourescence effects are minimal.  Under these assumptions, we can perform Cliff-Lorimer analysis.

Cliff Lorimer analysis assumes that the intensity of the observed peaks are correlated with the atomic abundance of their corresponding elements within the sample.

Ia/Ib = Kab * Ca/Cb

Ia and Ib are the size (number of X-ray counts) of the peaks corresponding to elements a and b in our sample.
Ca and Cb are the acutal elemental abundances of elements a and b in our sample.
Kab is a correction factor for relating the peak size and elemental abundances of elements a and b in our sample.

Kab is typically determined ahead of time through the study of samples of known composition.

This project aims to take a TEM-EDXS spectra, quantify the counts in each observed peak, and then relate those counts to elemental abundances using previously calculated Cliff-Lorimer K factors.

The user inputs a spectra and clicks on the spectra (CSV or Tab Delimited File) to indicate which peaks they wish to quantify.  Afterwards they input the elements and K factors needed for Cliff-Lorimer analysis.
