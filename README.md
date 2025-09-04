# Calibration Tools
These software tools are used to aid in the calibration of streak cameras.

## Bias Voltage Setting
The bias voltage setting tool finds the first and last n peaks of a streaked comb pulse, such as this one:

<img width="1697" height="1702" alt="40ns_1GHz" src="https://github.com/user-attachments/assets/e614a220-5db3-40ce-a24f-195efa28840e" />

The software tool then calculates the spacing between the peaks. The difference between the spacing of the first and last n peaks is calculated as a measure of sweep linearity. The bias voltage is adjusted until the difference calculation is approximately zero.

A plot of the lineout from which the calculations are taken highlights the peaks that were used for the calculation for the user to verify the correct peaks:

<img width="560" height="428" alt="Figure_1" src="https://github.com/user-attachments/assets/20528eec-1327-4d73-8a29-24c7b72180c8" />

## Contrast Transfer Ratio (CTR) Calculator
The CTR calculator assists with camera resolution evaluation during the calibration process. The image analyzed must be a flatfield with a Ronchi Ruling mask, such as this one:

<img width="1700" height="1702" alt="10s_FF_5lppmm_RR" src="https://github.com/user-attachments/assets/92bf7d3a-ccc5-44b1-96a5-0843017449f8" />

This tool produces CTR measurements throughout an image and retrieves specific measurements at points of interest:

<img width="516" height="438" alt="Figure_2" src="https://github.com/user-attachments/assets/a7810e05-7d69-4071-9908-61415e6b2d9d" />

## Full Width at Half Maximum (FWHM) Calculator
The FWHM Calculator assists with optical alignment and focus during the streak camera calibration process. The image analyzed must be taken with an overfilled slit. It may be either a swept image with a short-pulse laser or a static image such as this:

<img width="3412" height="412" alt="75ms_Exp" src="https://github.com/user-attachments/assets/b9b82a78-0f69-45ab-8bb0-8f2aa51d7972" />

This calibration tool fits a Gaussian curve to each line of the image and calculates the FWHM from the optimal hyperparameters, which it then displays as a graph.

It also produces measurements for the average FWHM of a 40-pixel swath at three points of interest along the image (25%, 50%, and 75% spatially), in accordance with procedure:

<img width="564" height="450" alt="Figure_3" src="https://github.com/user-attachments/assets/aabd7237-d926-4710-b6de-1b9a7ffd87c1" />
