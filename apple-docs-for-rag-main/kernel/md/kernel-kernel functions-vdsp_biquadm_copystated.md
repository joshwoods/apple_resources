

- Kernel
- Kernel Functions
-  vDSP_biquadm_CopyStateD 

Function

# vDSP_biquadm_CopyStateD

Copies the filter state from one dopuble-precision multichannel biquad IIR filter object to another.

macOS 10.10+

``` source
void vDSP_biquadm_CopyStateD(vDSP_biquadm_SetupD __dest, const struct vDSP_biquadm_SetupStructD *__src);
```

## Parameters 

`__dest`  

The `vDSP_biquadm_SetupD` object whose state you wish to overwrite.

`__src`  

The `vDSP_biquadm_SetupStructD` object whose state you wish to copy.

## Discussion

Both `src` and `dest` objects must be valid single-precision multichannel biquad setup objects created by previous calls to vDSP_biquadm_CreateSetupD. Both objects must have the same number of channels and sections.

