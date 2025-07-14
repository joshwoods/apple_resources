

- Accelerate
- vDSP
-  Multichannel biquadratic filters 

API Collection

# Multichannel biquadratic filters

Filter a multichannel signal with a cascade of biquadratic sections.

## Overview

The vDSP library implements biquadratic filtering as a cascade of individual infinite impulse response (IIR) filters called *sections.* Each section has its own set of feedback and feedforward coefficients, and implements a direct-form 2 filter.

When the biquadratic filter function executes, the sections execute in sequence. Each section processes the entire input signal and passes its output to the next section for further processing.

Note

The vDSP biquadratic filters work in place. That is, the source and destination pointers may point to the same memory.

Note on performance and energy efficiency

Although you can use vDSP_biquadm to process a single channel of data, it’s optimized for processing multiple channels of data independently. When processing only a single channel, the single-channel API vDSP_biquad may provide better performance and energy efficiency. When processing a single channel in isolation, it’s best practice to use vDSP_biquad whenever possible.

## Topics

### Equalizing audio with biquadratic filters

Equalizing audio with discrete cosine transforms (DCTs)

Change the frequency response of an audio signal by manipulating frequency-domain data.

### Creating a multichannel biquadratic filter setup

vDSP_biquadm_CreateSetup

Builds a data structure that contains precalculated data for use by a single-precision, multichannel cascaded biquadratic filter function.

typealias vDSP_biquadm_Setup

A data structure that contains precalculated data for use by a single-precision, multichannel cascaded biquadratic filter function.

vDSP_biquadm_CreateSetupD

Builds a data structure that contains precalculated data for use by a double-precision, multichannel cascaded biquadratic filter function.

typealias vDSP_biquadm_SetupD

A data structure that contains precalculated data for use by a double-precision, multichannel cascaded biquadratic filter function.

### Copying the filter state of a multichannel biquadratic filter

vDSP_biquadm_CopyState

Copies the filter state from one single-precision multichannel biquadratic IIR filter object to another.

vDSP_biquadm_CopyStateD

Copies the filter state from one double-precision multichannel biquadratic IIR filter object to another.

### Resetting the filter state of a multichannel biquadratic filter

vDSP_biquadm_ResetState

Resets the filter state of a single-precision multichannel biquadratic IIR filter object.

vDSP_biquadm_ResetStateD

Resets the filter state of a double-precision multichannel biquadratic IIR filter object.

### Setting the filter state of a multichannel biquadratic filter

vDSP_biquadm_SetActiveFilters

Activates or deactivates individual sections in a single-precision, multichannel biquadratic filter.

vDSP_biquadm_SetActiveFiltersD

Activates or deactivates individual sections in a double-precision, multichannel biquadratic filter.

### Setting the coefficients of a multichannel biquadratic filter

vDSP_biquadm_SetCoefficientsSingle

Sets the single-precision coefficients of the specified single-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetCoefficientsDouble

Sets the double-precision coefficients of the specified single-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetCoefficientsSingleD

Sets the single-precision coefficients of the specified double-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetCoefficientsDoubleD

Sets the double-precision coefficients of the specified double-precision, multichannel biquadratic filter setup object.

### Setting the target values of a multichannel biquadratic filter

vDSP_biquadm_SetTargetsSingle

Sets the single-precision coefficient target values of the specified single-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetTargetsDouble

Sets the double-precision coefficient target values of the specified single-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetTargetsSingleD

Sets the single-precision coefficient target values of the specified double-precision, multichannel biquadratic filter setup object.

vDSP_biquadm_SetTargetsDoubleD

Sets the double-precision coefficient target values of the specified double-precision, multichannel biquadratic filter setup object.

### Applying a multichannel biquadratic filter

vDSP_biquadm

Applies a single-precision multichannel biquadratic IIR filter.

vDSP_biquadmD

Applies a double-precision multichannel biquadratic IIR filter.

### Destroying a multichannel biquadratic filter setup

vDSP_biquadm_DestroySetup

Destroys a single-precision multichannel biquadratic filter setup object.

vDSP_biquadm_DestroySetupD

Destroys a double-precision multichannel biquadratic filter setup object.

## See Also

### Vector filtering

Biquadratic IIR filters

Apply biquadratic filters to single-channel and multichannel data.

Single-channel biquadratic filters

Filter a single-channel signal with a cascade of biquadratic sections.

Finite impulse response filters

Perform finite impulse response filtering with decimation and antialiasing on vectors of real or complex values.

Recursive filters

Perform two-pole two-zero recursive filtering on a vector.

