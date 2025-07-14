

- Kernel
- Kernel Functions
-  vDSP_biquadm_SetActiveFilters 

Function

# vDSP_biquadm_SetActiveFilters

Sets the overall active/inactive filter state of a valid single-precision multichannel biquad IIR filter setup of type `vDSP_biquadm_Setup`.

macOS 10.11+

``` source
void vDSP_biquadm_SetActiveFilters(vDSP_biquadm_Setup __setup, const bool *__filter_states);
```

## Parameters 

`__setup`  

The setup object to modify.

`__filter_states`  

An input array of `bool` values. The length of this array should be the number of filters configured in *setup*.

## Discussion

For each filter configured in `setup`, the corresponding value in `filter_states` sets the filter to its active or inactive state. The function removes any inactive filters from the biquad processing chain. The inactive filters retain their state if you activate them later.

