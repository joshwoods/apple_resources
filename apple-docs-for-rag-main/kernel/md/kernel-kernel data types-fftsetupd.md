

- Kernel
- Kernel Data Types
-  FFTSetupD 

Type Alias

# FFTSetupD

An opaque type that contains setup information for a given double-precision FFT transform.

macOS 10.13+

``` source
typedef struct OpaqueFFTSetupD *FFTSetupD;
```

## Discussion

A setup object can be allocated with vDSP_create_fftsetupD and destroyed with vDSP_destroy_fftsetupD. The setup object includes, among other things, precomputed tables used in computing an FFT of the specified size.

