# ERG
Scripts for electroretinography analysis
Two scripts are included, one for scotopic recordings, one for photopic recordings.
The main differences between the two scripts are:
- the acquisition frequency
- the time intervals in which the OPs are searched for
- the number of traces considered for the analysis : both protocols are using 3 flashes intensity, but practically only two intensities induced responses in the photopic protocol, and a single one in the scotopic protocol. In the "scotopic" script, the flat traces are dropped from the start. The "photopic" script has commented lines that can de activated to make it work with 3 intensities rather than 2.

Both scripts generate files containing the filtered traces (CSV format) and the coordinates of the OPs (time and amplitude) in Excel format. In the latter, the Time and Amplitude sheets contain respectively the time and amplitude of the four detected OPs (that is, for each of the four set time intervals, the peak with the largest positive amplitude). The third sheet called "Pics" contains the time and amplitude of each of the peaks detected in the 0-100 ms interval.
These peaks are labelled (red dots and numbers) on each filtered traces, so in case some of the automatically detected peaks are not considered as correct by the experimenter/analyser, or if more than four OPs are considered, the corresponding values can be looked for in "Pics". 
