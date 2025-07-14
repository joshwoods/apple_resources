

- Kernel
- AppleDSP
-  IIRChannel 

Type Alias

# IIRChannel

Constants that specify which channels a stereo biquadratic filter operates.

macOS 10.9+

``` source
typedef int IIRChannel;
```

## Discussion

Pass an `IIRChannel` constant to vDSP_biquad2_CreateSetup to specify which channels the function applies filtering to.

`vDSP_IIRStereo`  
The filter operates over both channels.

`vDSP_IIRMonoLeft`  
The filter operates on left-channel mono data and applies pass-through coefficients to the right channel.

`vDSP_IIRMonoRight`  
The filter operates on right-channel mono data and applies pass-through coefficients to the left channel.

## See Also

### Biquadratic Infinite Impulse Response (IIR) Filters

vDSP_biquad2

Applies a single-precision stereo biquadratic IIR filter.

vDSP_biquad2_CreateSetup

Builds a data structure that contains precalculated single-precision data for stereo biquadratic filter functions to use.

vDSP_biquad2_CopyState

Copies the filter state from one biquadratic filter object to another.

vDSP_biquad2_ResetState

Resets the filter state of a single-precision stereo biquadratic filter object.

vDSP_biquad2_DestroySetup

Destroys a single-precision stereo biquadratic IIR setup object.

