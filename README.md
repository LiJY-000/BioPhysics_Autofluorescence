# Autofluorescence


Background Research:

    Functional PCA (FPCA):
        R libraries: fda & fdapace
        Looked into FPCA with two x-axis values (time & wavelength)
        
    Other Signal Processing Methods:
        Tensor Decomposition for Signals - uses Tucker decomposition of tensors - could be applicable if we transform into tensors
        Linear Discriminant Analysis (LDA) - supervised dimensionality reduction - not applicable
        Independent Component Analysis (ICA) - used to decompose a multivariate signal - not applicable
        
    Comparing FPCA components:
        Visualize results with a scree plot and plots of eigenfunctions
        Interpret the patterns, variance explained, and scores from the FPCA output.
        Procrustes Analysis


Data Processing:

    Read in the example experiment (with 71 different files representing the temporal aspect) and combined them into 1 data frame. Also generated two data frames, one for before   chemical was added and another for after chemicals were added


Exploratory Data Analysis

    box plots & spectra plots for different times (all together, split between before and after adding the chemical, at certain times after the chemical has been added)


FPCA Fitting

    Three different FPCA methods to deal with time:
        FPCA for each of the 71 files
        FPCA for the spectra averaged before chemical was added and one for after chemicals were added
        FPCA for the spectra averaged across all time
