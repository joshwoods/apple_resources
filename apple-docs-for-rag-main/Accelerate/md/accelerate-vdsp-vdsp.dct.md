

- Accelerate
- vDSP
-  vDSP.DCT 

Class

# vDSP.DCT

A single-precision discrete cosine transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
class DCT
```

## Topics

### Initializers

init?(previous: vDSP.DCT?, count: Int, transformType: vDSP.DCTTransformType)

Initializes a new discrete cosine transform instance.

### Instance Methods

func transform&lt;U>(U) -> [Float]

Returns the single-precision real discrete cosine transform.

func transform&lt;U, V>(U, result: inout V)

Computes an out-of-place single-precision real discrete cosine transform.

## See Also

### Objects that Simplify Discrete Cosine Transforms

enum DCTTransformType

An enumeration that describes the discrete cosine transform types.

