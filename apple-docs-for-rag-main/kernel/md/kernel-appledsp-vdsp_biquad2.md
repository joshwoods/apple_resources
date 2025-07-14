

- Kernel
- AppleDSP
-  vDSP_biquad2 

Function

# vDSP_biquad2

Applies a single-precision stereo biquadratic IIR filter.

macOS 10.9+

``` source
void vDSP_biquad2(const struct vDSP_biquad_SetupStruct *, const float *, float *, size_t);
```

## Parameters 

`Parameter 0`  

The data structure that stores the biquadratic filter state and coefficients.

`Parameter 1`  

A pointer to the single-precision interleaved stereo input data.

`Parameter 2`  

A pointer to the single-precision interleaved stereo output data.

`Parameter 3`  

The number of elements per channel.

## Discussion

Use this function to apply a stereo biquadratic IIR filter to the input and write the filtered result to the output. The input and output are interleaved so that even elements correspond to the left channel and odd elements correspond to the right channel.

## See Also

### Biquadratic Infinite Impulse Response (IIR) Filters

vDSP_biquad2_CreateSetup

Builds a data structure that contains precalculated single-precision data for stereo biquadratic filter functions to use.

IIRChannel

Constants that specify which channels a stereo biquadratic filter operates.

vDSP_biquad2_CopyState

Copies the filter state from one biquadratic filter object to another.

vDSP_biquad2_ResetState

Resets the filter state of a single-precision stereo biquadratic filter object.

vDSP_biquad2_DestroySetup

Destroys a single-precision stereo biquadratic IIR setup object.

