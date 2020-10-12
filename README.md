**Calculate the power spectrum of data taken on BL4A (MagRef)**

This code calculates the power spectrum of event mode data collected with ns accuracy on BL4A (MagRef) at the SNS, ORNL. Care was taken to ensure adequate numerical precision of the event timing. The code essentially calculates the discrete Fourier transform of the event stream and from this the power spectrum. A run of example data is provided.

To obtain the power spectrum execute the following steps:

1. Define a working directory
2. In this directory make a sub-directory called &quot;input&quot;
3. In /input put the NumPy binary files of event mode data and metadata logs obtained using the Jupyter notebook &quot;BL4A\_get\_single\_event\_batch&quot; [T.R. Charlton and M.R. Fitzsimmons, _Code to obtain single event data from Spallation Neutron Source Beamline-4A (MagRef)_ (2020) [https://doi.org/10.5281/zenodo.3967680](https://doi.org/10.5281/zenodo.3967680)]
4. Run the Jupyter notebook &quot;AutoCorrelation\_batch&quot; after making changes to the code as instructed in the notebook. This notebook produces a set of files tagged with &quot;\_power&quot;. Each file contains 2 columns: frequency (Hz) and power spectrum. The first line of the output also includes the total number of events observed, and the count rate (over the whole detector).

Work funded by the U.S. Department of Energy under contract No. DE-AC05-00OR22725.

M.R. Fitzsimmons (10.12.2020)