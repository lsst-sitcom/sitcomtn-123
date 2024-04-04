#####################################################
TMA Capacitor Bank discharge vs Acceleration profiles
#####################################################

.. abstract::

   Continue the analysis started in SITCOM-1146. Based on the input from a team review, focusing on aspects below. Another ticket opened to investigate current draw profiles.

Relationship of min power supply voltage and distance of slew

Explore when Az and El moved at same time, rather than separately

Look at Azimuth acceleration vs. power supply voltage


Introduction
=============
The contractor responsible for the TMA Power supply and capacitor banks, Phase, has indicated that it is best to keep the voltage drops during a slew to above 575 V. Excessive loss of power from the TMA could lead to poor performance of observations due to the telescope not being able to move properly. In this analysis we have followed the one performed on the `SITCOM-1146 <https://rubinobs.atlassian.net/browse/SITCOM-1146>`_, identifying each slew of the observation nights using `TMAEventMaker()`. Selecting:

::

  lsst.sal.MTMount.mainPowerSupply
  lsst.sal.MTMount.elevation
  lsst.sal.MTMount.azimuth


These tests analyze what is the min power supply voltage along the different movements that the telescope performs during slew (analizing their velocities and acceleration) and if in some positions or concrete movements could suggest problems. We explore the minimum `powerSupplyVoltage` as a function of slew distance, as well as the behavior during velocity and acceleration. We also explore when the telescope moves in azimuth and elevation at the same time and when it moves separately.

Results have been analyzed for observing nights 20240220 and 20240221. During these dates it was not possible to accelerate the telescope so the final results of this analysis are pending observational data. 


Related Tickets
================
* `SITCOM-1146 <https://rubinobs.atlassian.net/browse/SITCOM-1146>`_: *TMA Performance Settings vs Capacitor Bank discharge*


Related Requirements
=====================
* Voltage drops during a slew must remain above 575 V.






Add content here
================

See the `Documenteer documentation <https://documenteer.lsst.io/technotes/index.html>`_ for tips on how to write and configure your new technote.
