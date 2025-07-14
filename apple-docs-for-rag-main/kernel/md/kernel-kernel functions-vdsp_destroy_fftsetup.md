

- Kernel
- Kernel Functions
-  vDSP_destroy_fftsetup 

Function

# vDSP_destroy_fftsetup

Deallocates an existing single-precision FFT setup structure.

macOS 10.0+

``` source
void vDSP_destroy_fftsetup(FFTSetup __setup);
```

## Parameters 

`__setup`  

The setup structure to deallocate, previously created by vDSP_create_fftsetup.

## Discussion

`vDSP_destroy_fftsetup` frees existing setup data and releases any allocated memory.

