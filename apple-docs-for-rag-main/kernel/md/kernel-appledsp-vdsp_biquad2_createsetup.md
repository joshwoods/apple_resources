

- Kernel
- AppleDSP
-  vDSP_biquad2_CreateSetup 

Function

# vDSP_biquad2_CreateSetup

Builds a data structure that contains precalculated single-precision data for stereo biquadratic filter functions to use.

macOS 10.9+

``` source
vDSP_biquad_Setup vDSP_biquad2_CreateSetup(const double *, const size_t, const IIRChannel);
```

## Parameters 

`Parameter 0`  

A pointer to the double-precision filter coefficients.

`Parameter 1`  

The number of sections in the biquadratic filter.

`Parameter 2`  

An enumeration that specifies the channel.

## Discussion

If the channel parameter is `vDSP_IIRMonoLeft` or `vDSP_IIRMonoRight`, the number of elements in the coefficients array must be five times the number of sections. The filter applies pass-through coefficients to the other channel.

If the channel parameter is `vDSP_IIRStereo`, the number of elements in the coefficients array must be ten times the number of sections. Specify five left-channel coefficients followed by five right-channel coefficients.

## See Also

### Biquadratic Infinite Impulse Response (IIR) Filters

vDSP_biquad2

Applies a single-precision stereo biquadratic IIR filter.

IIRChannel

Constants that specify which channels a stereo biquadratic filter operates.

vDSP_biquad2_CopyState

Copies the filter state from one biquadratic filter object to another.

vDSP_biquad2_ResetState

Resets the filter state of a single-precision stereo biquadratic filter object.

vDSP_biquad2_DestroySetup

Destroys a single-precision stereo biquadratic IIR setup object.

