# CMN-Temperature-Calibration-and-Sensing
Because the CMN sensor lacks a calibration curve and Cernox sensors are inaccurate below ~100mK, I first calibrated the CMN resistance against the Cernox temperature in the overlapping functional regime. Using this calibration, I extrapolated the CMN resistance to measure temperatures as the Cernox sensor becomes undeterable.

The temperature vs CMN resistance is supposed to follow:

$T = \frac{C}{Q - Q_0}$, 

where C and $Q_0$ are fixed parameters, Q is CMN resistance, and T is temperature. 

To run the script, execute 'Temperature_Log.ipynb' sequentially from top to bottom. The required files are 'Q9_T.csv' and 'time_Q9.csv'. 

* Q9_T.csv: Used for CMN calibration. It contains two columns with headers -- the 1st column is CMN resistance (Q9) [mOhm], and the 2nd column is temperatue T [K].
* time_Q9.csv: Record Q9 over time.

After execution, the script generates 'temperature_log.csv' which contains four columns: Time, Q9 [mOhm], T [K], and sigma_T [K] (the uncertainty of the calculated temperature).
