

- Kernel
- Kernel Functions
-  vDSP_biquadm_SetCoefficientsSingle 

Function

# vDSP_biquadm_SetCoefficientsSingle

Updates single-precision coefficients within a valid single-precision multichannel biquad IIR filter object.

macOS 10.11+

``` source
void vDSP_biquadm_SetCoefficientsSingle(vDSP_biquadm_Setup __setup, const float *__coeffs, vDSP_Length __start_sec, vDSP_Length __start_chn, vDSP_Length __nsec, vDSP_Length __nchn);
```

## Parameters 

`__setup`  

The filter state object whose coefficients you wish to update.

`__coeffs`  

An input array of single-precision coefficients.

`__start_sec`  

First section to update in each channel.

`__start_chn`  

First channel to update.

`__nsec`  

Number of sections to update in each channel.

`__nchn`  

Number of channels to update.

## Discussion

Use this function to update sections of coefficient values of a biquad setup structure. This function doesn’t allocate new memory. The range specified by `__start_sec` and `__nsec` must be within the number of sections defined by the create setup function.

