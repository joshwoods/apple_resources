

- Kernel
- Kernel Functions
-  vDSP_biquadm_CopyState 

Function

# vDSP_biquadm_CopyState

Copies the filter state from one single-precision multichannel biquad IIR filter object to another.

macOS 10.9+

``` source
void vDSP_biquadm_CopyState(vDSP_biquadm_Setup __dest, const struct vDSP_biquadm_SetupStruct *__src);
```

## Parameters 

`__dest`  

The `vDSP_biquadm_Setup` object whose state you wish to overwrite.

`__src`  

The `vDSP_biquadm_SetupStruct` object whose state you wish to copy.

## Discussion

Both `src` and `dest` objects must be valid single-precision multichannel biquad setup objects created by previous calls to vDSP_biquadm_CreateSetup. Both objects must have the same number of channels and sections.

