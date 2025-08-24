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
