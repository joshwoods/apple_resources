

- Accelerate
- vDSP
-  taperedMerge(\_:\_:) 

Type Method

# taperedMerge(\_:\_:)

Returns the result of a tapered merge between two single-precision vectors.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func taperedMerge(
    _ vectorA: T,
    _ vectorB: U
) -> [Float] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Float, U.Element == Float
```

## Parameters 

`vectorA`  

The first vector to merge.

`vectorB`  

The second vector to merge.

## Return Value

The result of the tapered merge operation.

## Discussion

The following code performs a tapered merge between two vectors that represent sine waves at different frequencies:

```
let count = 1024

let vectorA: [Float] = (0 ..

The following image shows the result of the tapered merge in `tapered`.

## See Also

### Vector-to-vector merging functions

static func taperedMerge&lt;T, U>(T, U) -> [Double]

Returns the result of a tapered merge between two double-precision vectors.

static func taperedMerge&lt;T, U, V>(T, U, result: inout V)

Computes the result of a tapered merge between two single-precision vectors.

static func taperedMerge&lt;T, U, V>(T, U, result: inout V)

Computes the result of a tapered merge between two double-precision vectors.

