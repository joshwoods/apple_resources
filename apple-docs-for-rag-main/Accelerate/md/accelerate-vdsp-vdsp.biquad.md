

- Accelerate
- vDSP
-  vDSP.Biquad 

Structure

# vDSP.Biquad

A single- or double-precision biquadratic filter.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct Biquad where T : vDSP_FloatingPointBiquadFilterable
```

## Overview

Note

The vDSP biquadratic filters work in place. That is, the source and destination pointers may point to the same memory.

## Topics

### Initializers

init?(coefficients: [Double], channelCount: vDSP_Length, sectionCount: vDSP_Length, ofType: T.Type)

Creates a new single-channel or multichannel cascaded biquad IIR structure.

### Instance methods

func apply&lt;U>(input: U) -> [T]

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, returning the filtered signal.

func apply&lt;U, V>(input: U, output: inout V)

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, overwriting the supplied output vector.

## See Also

### Biquadratic IIR Filters

Equalizing audio with discrete cosine transforms (DCTs)

Change the frequency response of an audio signal by manipulating frequency-domain data.

