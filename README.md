# chronoamp-analysis
Template code that analyzes chronoamperometry data from an excel file exported from PSTrace.

Creates three plots:
Plot 1: Raw current vs. time for each trial
  Verify that this plot matches the plot you observed in PSTrace.
Plot 2: Averaged current vs. time for each concentration
  Useful figure to include in reports or journal articles. Demonstrates time-resolved current behavior at each analyte concentration.
Plot 3: Calibration curve (current vs. concentration with linear fit)
  Shows sensitivity and linearity of your system. Slope is printed to the MATLAB console.

Be sure to adjust the following to reflect your experiment:
Number of trials
Concentrations used
Plot titles and Axes

Troubleshooting notes:
Make sure that this script and your excel file are in the same directory.
Adjust number of trials and concentrations to reflect your data
For plot 3, to get one current measurement for each trial, the current from t = 100s to t = 110s is averaged, which is recommended. However, this can be manipulated within reason if needed.
Verify the units from your raw data: Concentration should be in mmol and current should be in μA (should be the PSTrace default) for the code to work as intended. If not, adjust the conversion factors in the code.
