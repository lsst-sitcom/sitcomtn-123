.. image:: https://img.shields.io/badge/sitcomtn--123-lsst.io-brightgreen.svg
   :target: https://sitcomtn-123.lsst.io
.. image:: https://github.com/lsst-sitcom/sitcomtn-123/workflows/CI/badge.svg
   :target: https://github.com/lsst-sitcom/sitcomtn-123/actions/

#####################################################
TMA Capacitor Bank discharge vs Acceleration profiles
#####################################################

SITCOMTN-123
============

Continue the analysis started in SITCOM-1146. Based on the input from a team review, focusing on aspects below. Another ticket opened to investigate current draw profiles.

Relationship of min power supply voltage and distance of slew

Explore when Az and El moved at same time, rather than separately

Look at Azimuth acceleration vs. power supply voltage

Results and analysis to be added to SITCOMTN-110

**Links:**

- Publication URL: https://sitcomtn-123.lsst.io
- Alternative editions: https://sitcomtn-123.lsst.io/v
- GitHub repository: https://github.com/lsst-sitcom/sitcomtn-123
- Build system: https://github.com/lsst-sitcom/sitcomtn-123/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

.. code-block:: bash

   git clone https://github.com/lsst-sitcom/sitcomtn-123
   cd sitcomtn-123
   make init
   make html

Repeat the ``make html`` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run ``make clean``.

The built technote is located at ``_build/html/index.html``.

Publishing changes to the web
=============================

This technote is published to https://sitcomtn-123.lsst.io whenever you push changes to the ``main`` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://sitcomtn-123.lsst.io/v.

Editing this technical note
===========================

The main content of this technote is in ``index.rst`` (a reStructuredText file).
Metadata and configuration is in the ``technote.toml`` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
