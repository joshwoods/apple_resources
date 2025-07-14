

- Accelerate
-  Discrete Cosine transforms 

API Collection

# Discrete Cosine transforms

Transform vectors of temporal and spatial domain real values to the frequency domain, and vice versa.

## Topics

### First Steps

Signal extraction from noise

Use Accelerate’s discrete cosine transform to remove noise from a signal.

Equalizing audio with discrete cosine transforms (DCTs)

Change the frequency response of an audio signal by manipulating frequency-domain data.

### Objects that Simplify Discrete Cosine Transforms

class DCT

A single-precision discrete cosine transform.

enum DCTTransformType

An enumeration that describes the discrete cosine transform types.

### Discrete Cosine Transforms

The functions in the Discrete Cosine Transforms (DCT) family calculate a discrete cosine transform of a specified length on a vector.

vDSP_DCT_CreateSetup

Builds a data structure that contains precalculated data to perform a discrete cosine transform.

enum vDSP_DCT_Type

Constants that indicate the type for a discrete cosine transform.

vDSP_DCT_Execute

Calculates the discrete cosine transform for a vector.

## See Also

### Fourier and Cosine Transforms

Understanding data packing for Fourier transforms

Format source data for the vDSP Fourier functions, and interpret the results.

Finding the component frequencies in a composite sine wave

Use 1D fast Fourier transform to compute the frequency components of a signal.

Performing Fourier transforms on interleaved-complex data

Optimize discrete Fourier transform (DFT) performance with the vDSP interleaved DFT routines.

Reducing spectral leakage with windowing

Multiply signal data by window sequence values when performing transforms with noninteger period signals.

Signal extraction from noise

Use Accelerate’s discrete cosine transform to remove noise from a signal.

Performing Fourier Transforms on Multiple Signals

Use Accelerate’s multiple-signal fast Fourier transform (FFT) functions to transform multiple signals with a single function call.

Halftone descreening with 2D fast Fourier transform

Reduce or remove periodic artifacts from images.

Fast Fourier transforms

Transform vectors and matrices of temporal and spatial domain complex values to the frequency domain, and vice versa.

Discrete Fourier transforms

Transform vectors of temporal and spatial domain complex values to the frequency domain, and vice versa.

