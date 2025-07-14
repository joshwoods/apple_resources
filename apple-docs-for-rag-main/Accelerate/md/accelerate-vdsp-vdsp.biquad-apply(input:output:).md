

- Accelerate
- vDSP
- vDSP.Biquad
-  apply(input:output:) 

Instance Method

# apply(input:output:)

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, overwriting the supplied output vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
mutating func apply(
    input: U,
    output: inout V
) where T == U.Element, U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == V.Element
```

## See Also

### Instance methods

func apply&lt;U>(input: U) -> [T]

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, returning the filtered signal.

