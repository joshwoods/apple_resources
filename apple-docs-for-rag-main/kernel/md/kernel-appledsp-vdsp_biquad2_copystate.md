

- Kernel
- AppleDSP
-  vDSP_biquad2_CopyState 

Function

# vDSP_biquad2_CopyState

Copies the filter state from one biquadratic filter object to another.

macOS 10.9+

``` source
void vDSP_biquad2_CopyState(vDSP_biquad_Setup, vDSP_biquad_Setup);
```

## Parameters 

`Parameter 0`  

The destination biquadratic filter object.

`Parameter 1`  

The source biquadratic filter object.

## See Also

### Biquadratic Infinite Impulse Response (IIR) Filters

vDSP_biquad2

Applies a single-precision stereo biquadratic IIR filter.

vDSP_biquad2_CreateSetup

Builds a data structure that contains precalculated single-precision data for stereo biquadratic filter functions to use.

IIRChannel

Constants that specify which channels a stereo biquadratic filter operates.

vDSP_biquad2_ResetState

Resets the filter state of a single-precision stereo biquadratic filter object.

vDSP_biquad2_DestroySetup

Destroys a single-precision stereo biquadratic IIR setup object.

