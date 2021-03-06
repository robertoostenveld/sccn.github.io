---
layout: default
title: Two decades of EEGLAB
long_title: The first two decades of EEGLAB
parent: EEGLAB news
---
The first two decades of EEGLAB
===

EEGLAB (v0.9) was first released on April 23, 2001 - thus, EEGLAB is now 20 years old!

![right](/assets/images/EEGLAB10years.jpg)

A bit of history
----------------

In 1997, Scott Makeig, Tzyy Ping Jung, and colleagues released the
ICA Electrophysiology Toolbox for MATLAB from Terrence Sejnowski's CNL
laboratory at The Salk Institute for Biological Studies in La Jolla.
This toolbox comprised functions to run (extended) infomax ICA on EEG
data as well as early versions of time/frequency and visualization
functions used in EEGLAB including eegplot(), topoplot(), headplot(),
envtopo(), timtopo(), and erpimage(). In 2000, Arnaud Delorme
joined the Salk Institute and wrote the first version of EEGLAB to reject
automatically (or semi-automatically) artifacts in EEG data. This
version of EEGLAB used the ICA toolbox mentioned above for some of the data processing. We demonstrate
below how the current version of EEGLAB remains backward compatible with
this very early version of EEGLAB (v0.9). EEGLAB versions 1 and 2
followed. *EEGLAB v2*, released in 2002, implemented the EEGLAB
history feature that users can use to generate EEGLAB scripts automatically. Scripts generated by this version are still compatible with the
current EEGLAB version.

By 2001, the team of researchers working on EEG processing in Terrence Sejnowski's CNL
laboratory (including Dr. Delorme and Makeig) was becoming too large for the space available.
Coincidentally, Dr. Jerome Swartz, an early inventor of laser barcoding,
agreed to give funds to UCSD to create a research center dedicated to
studies of higher-order human cognition using EEG. Based on the
initiative of Terry Sejnowski, the
Swartz Center for Computational Neuroscience (SCCN) was founded under
the then-small Institute of Neural Computation at UCSD. Scott Makeig became the director of this new center, and Dr. Arnaud Delorme and other EEG researchers also moved from the Salk Institute to the new center.

At SCCN, command-line functions of the ICA Electrophysiology toolbox and
the proto version of EEGLAB were fused. *EEGLAB v3*, an internal version,
was never released. *EEGLAB v4*, the first integrated and fully
functional version of EEGLAB, was released at the end of 2002.

Several revisions of EEGLAB v4 were released from 2003 to 2006,
strengthening the code and adding capabilities for importing data in
many different formats. In 2006, *EEGLAB v5* was released, adding
the STUDY structure and many functions giving EEGLAB users a pipeline
for processing data from multiple subjects, including the first software
for ICA component clustering.

In 2007, *EEGLAB v6* was released, allowing users to perform
statistical analyses at the STUDY level and use EEGLAB plugins.

In 2009, *EEGLAB v7* was released under a new revision control
system (migrated from RCS to CVS) that added consistency and reliability.

At the beginning of 2010, *EEGLAB v8* was released, allowing access
to single-trial subsets from STUDY functions.

At the end of 2018, a new version of EEGLAB was released that offered full support for single-trial analyses. This version also contained the EEGLAB plugin manager.

More details about each EEGLAB
version is available on the [EEGLAB revision
page](/others/EEGLAB_revision_history.html).

Statistics
----------
The total
number of lines of code (excluding plugins) is currently 145,271
comprising 636 stand-alone functions. Currently, there are 15,265 researchers on
the EEGLAB news list. EEGLAB has been downloaded about 350,000 times. According to the ISI web of knowledge, the
original 2004 [EEGLAB
paper](http://sccn.ucsd.edu/eeglab/download/eeglab_jnm03.pdf) has been
cited 14,400 times.

EEGLAB is still backward compatible with EEGLAB v0.9
-----------------------------------------------------
This section is just for fun! Below we illustrate how serious we are about backward compatibility, showing that files saved with EEGLAB v0.9 can still be read in EEGLAB version 2021.

You may download below the original files for the first version of EEGLAB
released on April 23, 2001 (full instructions are also available on the
original EEGLAB [web page](http://sccn.ucsd.edu/~arno/eeglab.html)).
Please download and uncompress the archives of the EEGLAB, the ICA toolbox, and the test file.
-   [eeglab0.9.tar.gz](http://sccn.ucsd.edu/eeglab/download/eeglab0.9.tar.gz)
    (\< 1Mb)
-   [ica5.tar.gz](http://sccn.ucsd.edu//eeglab/download/ica5.tar.gz) (\<
    1Mb)
-   [TESTEEG.eeg](http://sccn.ucsd.edu/eeglab/download/TESTEEG.eeg) (50
    Mb)

Start MATLAB, add the path to each of the uncompressed folders, and type *\>\>eeglab* on the command line.

![EEGLAB v0.9 graphic interface](/assets/images/EEGLAB0_9.png)

Then select the <span style="color: brown">File → Load EEG</span> menu item. Select the "TESTEEG.eeg" file you
have downloaded. Be sure to change the default event type range from *12501:12600* to *all*, as shown in the image below.

![left\|150px](/assets/images/Eeglab09_load.png)

EEGLAB loads the dataset and plots an ERP-image figure (it will also generate an error under MATLAB 2020a because of axes settings incompatibility - remember this version is 20 years old!). You may use <span style="color: brown">Plot → average</span> to pop up the plot below.

![left\|150px](/assets/images/eeglab09_plot.png)


You
may then save the dataset using the <span style="color: brown">File → Save set</span> menu item.

Then go back to your current version of EEGLAB: remove the paths to
EEGLAB v0.9 and restart your current version of EEGLAB. Load and manipulate the dataset you
have just saved in EEGLAB v0.9.

![left\|150px](/assets/images/eeglab2021test.png)

This exercise demonstrates how, since the beginning of EEGLAB, we have
maintained backward compatibility between EEGLAB versions
(supported by the relative stability of MATLAB itself).

<i>Arnaud Delorme, January 6, 2021</i>