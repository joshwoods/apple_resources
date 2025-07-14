

- Accelerate
- vDSP
-  swapElements(\_:\_:) 

Type Method

# swapElements(\_:\_:)

Swaps the elements of two single-precision vectors.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func swapElements(
    _ vectorA: inout T,
    _ vectorB: inout U
) where T : AccelerateMutableBuffer, U : AccelerateMutableBuffer, T.Element == Float, U.Element == Float
```

## Parameters 

`vectorA`  

The first vector.

`vectorB`  

The second vector.

## Discussion

The following code swaps the elements in `vectorA` with those in `vectorB`:

```
var vectorA: [Float] = [1, 3, 5, 7]
var vectorB: [Float] = [2, 4, 6, 8]

vDSP.swapElements(&vectorA,
                  &vectorB)

// Prints "[2.0, 4.0, 6.0, 8.0]".
print(vectorA)

// Prints "[1.0, 3.0, 5.0, 7.0]".
print(vectorB)
```

## See Also

### Vector-to-vector element swapping functions

static func swapElements&lt;T, U>(inout T, inout U)

Swaps the elements of two double-precision vectors.

