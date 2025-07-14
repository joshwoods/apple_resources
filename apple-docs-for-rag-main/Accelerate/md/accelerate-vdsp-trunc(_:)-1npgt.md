

- Accelerate
- vDSP
-  trunc(\_:) 

Type Method

# trunc(\_:)

Returns a single-precision array containing each element in the supplied vector truncated to a fraction.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func trunc(_ vector: U) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## See Also

### Single-Vector Fractional Part Extraction

static func trunc&lt;U>(U) -> [Double]

Returns a double-precision array containing each element in the supplied vector truncated to a fraction.

static func trunc&lt;U, V>(U, result: inout V)

Calculates each element in the supplied double-precision vector truncated to a fraction.

static func trunc&lt;U, V>(U, result: inout V)

Calculates each element in the supplied single-precision vector truncated to a fraction.

