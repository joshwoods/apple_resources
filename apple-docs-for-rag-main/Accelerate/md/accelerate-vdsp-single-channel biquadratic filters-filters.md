

- Accelerate
- vDSP
-  Single-channel biquadratic filters 

API Collection

# Single-channel biquadratic filters

Filter a single-channel signal with a cascade of biquadratic sections.

## Overview

The vDSP library implements biquadratic filtering as a cascade of individual infinite impulse response (IIR) filters called *sections.* Each section has its own set of feedback and feedforward coefficients, and implements a direct-form 1 filter.

When the biquadratic filter function executes, the sections execute in sequence. Each section processes the entire input signal and passes its output to the next section for further processing.

Note

The vDSP biquadratic filters work in place. That is, the source and destination pointers may point to the same memory.

## Topics

### Biquadratic filter essentials

Applying biquadratic filters to a music loop

Change the frequency response of an audio signal using a cascaded biquadratic filter.

Creating an audio unit extension using the vDSP library

Add biquadratic filter audio-effect processing to apps like Logic Pro X and GarageBand with the Accelerate framework.

### Creating a single-channel biquadratic filter setup

vDSP_biquad_CreateSetup

Builds a data structure that contains precalculated data for use by a single-precision cascaded biquadratic filter function.

typealias vDSP_biquad_Setup

A data structure that contains precalculated data for use by the single-precision cascaded biquadratic IIR filter function.

vDSP_biquad_CreateSetupD

Builds a data structure that contains precalculated data for use by a double-precision cascaded biquadratic filter function.

typealias vDSP_biquad_SetupD

A data structure that contains precalculated data for use by the double-precision cascaded biquadratic IIR filter function.

### Applying a single-channel biquadratic filter

vDSP_biquad

Applies a single-precision single-channel biquadratic IIR filter.

vDSP_biquadD

Applies a double-precision single-channel biquadratic IIR filter.

### Setting the coefficients of a single-channel biquadratic filter

vDSP_biquad_SetCoefficientsSingle

Sets single-precision coefficients of the specified single-channel biquadratic filter setup object.

vDSP_biquad_SetCoefficientsDouble

Sets double-precision coefficients of the specified single-channel biquadratic filter setup object.

### Destroying a single-channel biquadratic filter setup

vDSP_biquad_DestroySetup

Destroys a single-precision biquadratic filter setup object.

vDSP_biquad_DestroySetupD

Destroys a double-precision biquadratic filter setup object.

## See Also

### Vector filtering

Biquadratic IIR filters

Apply biquadratic filters to single-channel and multichannel data.

Multichannel biquadratic filters

Filter a multichannel signal with a cascade of biquadratic sections.

Finite impulse response filters

Perform finite impulse response filtering with decimation and antialiasing on vectors of real or complex values.

Recursive filters

Perform two-pole two-zero recursive filtering on a vector.

