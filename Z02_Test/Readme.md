<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/ziggle/BatteryDischargeQuickLookReport">
    <img src="../Images/components_Coin-cells.jpg" alt="Logo" width="511" height="363">

  </a>

<h1 align="center">Lithium-Ion Coin Cell Test Data</h1>

  <p align="center">
    I am analyzing battery discharge data using Python and Excel to illustrate how to perform the analysis.
    <br />
    <br />
    <a href="https://en.wikipedia.org/wiki/Button_cell">Image Source</a>
    ·
    <a href="https://en.wikipedia.org/wiki/Button_cell">Wikipedia Coin Cell Discussion</a>
  </p>
</div>

## Overview

This file contains results from capacity testing of 10.5 mA-hr (nominal) Lithium-ion coin cells on the Maccor battery tester. My initial test work was focused on simple capacity testing. I also plan to begin cycle testing with simulated customer profiles.

HW Engineering has requested that I also begin characterizing the behavior of the AC impedance versus cycle number. The battery impedance is an important charactristic with respect to battery's surge handling capabiities. Historically, HW Engineering has measured it, but they have requested that I measure during my testing since I have a setup that can easily add this measurement.

## Fixturing

My key challenge is building a fixture for testing a batch of batteries. The batteries are so small that I cannot use a standard fixture. I have some thinking to do about this.

## Test Data Dictionary

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
