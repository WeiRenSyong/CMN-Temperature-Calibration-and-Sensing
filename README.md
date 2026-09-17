# CMN-Temperature-Calibration-and-Sensing
Because the CMN sensor lacks a calibration curve and Cernox sensors are inaccurate below ~100mK, I first calibrated the CMN resistance against the Cernox temperature in the overlapping functional regime. Using this calibration, I extrapolated the CMN resistance to measure temperatures as the Cernox sensor becomes undeterable.

The temperature vs CMN resistance is supposed to follow:

$T = \frac{C}{Q - Q_0}$, 

where C and $Q_0$ are fixed parameters, Q is CMN resistance, and T is temperature. 