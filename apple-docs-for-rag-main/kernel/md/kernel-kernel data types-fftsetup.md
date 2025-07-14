

- Kernel
- Kernel Data Types
-  FFTSetup 

Type Alias

# FFTSetup

An opaque type that contains setup information for a given FFT transform.

macOS 10.13+

``` source
typedef struct OpaqueFFTSetup *FFTSetup;
```

## Discussion

A setup object can be allocated with vDSP_create_fftsetup and destroyed with vDSP_destroy_fftsetup. The setup object includes, among other things, precomputed tables used in computing an FFT of the specified size.

