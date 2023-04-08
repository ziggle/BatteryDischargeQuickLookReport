# Battery Test Results

This file contains results from capacity testing of 10.5 mA-hr (nominal) Lithium-ion coin cells on the Maccor battery tester

# Test Data Dictionary

There are many columns in the data, but only the following are used in the analysis.

- Cyc<br/>Battery tests are repeated multiple times. This is the particular iteration of the battery test.
- Step<br/>Battery tests consist of multiple steps, include rest, discharge, charge, and impedance test.
- Test Time<br/>The overall test time with a start time of "0d 00:00:00".
- Step Time<br/>The time spent in a specific step with a format of "0d 00:00:00".
- Amp-hr<br/>The amount of charge received/delivered during this step.
- Amps<br/>The charge delivered to or received from the battery under test.
- Volts<br/>The battery cell voltage.
- State</br/>A letter-based version of the step.
- AC Imp<br/>The AC impedance measure during the AC impedance step.
