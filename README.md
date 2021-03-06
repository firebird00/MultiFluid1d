MultiFluid1d
============

Simple code for time domain simulations of the two-stream instability in relativistic multifluids.

This is a (considerably tidied and slightly simplified) version of the 1+1 dimensional code used in the paper
"The nonlinear development of the relativistic two-stream instability", Hawke, Comer, Andersson (arXiV:1303.4070).

For historical reasons the master function used in the original code was considerably more complex (and messy). The version implemented here is that presented in the paper. The results are qualitatively similar, but the unstable results are quantitatively very slightly different as the instability depends on effects triggered near floating point error level.

The code has been tested with gfortran 4.6.* and Intel fortran 12.1.3 on Linux machines. 

Note that the core of the code is dimension independent and trivial to extend to higher dimensions (and the extension to 2+1 dimensions has been implemented and tested; as mentioned in the paper, no physically interesting results arise, due to the coupling timescales involved).

This code relies on the LAPACK library for matrix inversion, the FFTW3 library for Fourier transforms, and the minpack library for root-finding. Please see the disclaimer in the minpack directory for the terms of use of minpack - the original code can be found at netlib.org. The remaining files are licensed under the Creative Commons Attribution 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/.

