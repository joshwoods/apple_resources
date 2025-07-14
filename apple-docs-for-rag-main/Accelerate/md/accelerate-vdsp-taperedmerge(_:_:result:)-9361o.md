

- Accelerate
- vDSP
-  taperedMerge(\_:\_:result:) 

Type Method

# taperedMerge(\_:\_:result:)

Computes the result of a tapered merge between two double-precision vectors.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func taperedMerge(
    _ vectorA: T,
    _ vectorB: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Double, U.Element == Double, V.Element == Double
```

## Parameters 

`vectorA`  

The first vector to merge.

`vectorB`  

The second vector to merge.

`result`  

The destination vector that receives the result.

## Discussion

The following code performs a tapered merge between two vectors that represent sine waves at different frequencies:

```
let count = 1024

let vectorA: [Double] = (0 ..

The following image shows the result of the tapered merge in `tapered`.

## See Also

### Vector-to-vector merging functions

static func taperedMerge&lt;T, U>(T, U) -> [Float]

Returns the result of a tapered merge between two single-precision vectors.

static func taperedMerge&lt;T, U>(T, U) -> [Double]

Returns the result of a tapered merge between two double-precision vectors.

static func taperedMerge&lt;T, U, V>(T, U, result: inout V)

Computes the result of a tapered merge between two single-precision vectors.

