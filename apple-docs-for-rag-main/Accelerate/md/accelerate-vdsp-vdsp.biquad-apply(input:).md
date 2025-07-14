

- Accelerate
- vDSP
- vDSP.Biquad
-  apply(input:) 

Instance Method

# apply(input:)

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, returning the filtered signal.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
mutating func apply(input: U) -> [T] where T == U.Element, U : AccelerateBuffer
```

## See Also

### Instance methods

func apply&lt;U, V>(input: U, output: inout V)

Applies a single- or double-precision single-channel or multichannel biquad IIR filter, overwriting the supplied output vector.

