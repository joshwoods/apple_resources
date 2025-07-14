

- Core ML
- MLTensor
-  bandPart(lowerBandCount:upperBandCount:) 

Instance Method

# bandPart(lowerBandCount:upperBandCount:)

Returns a new tensor with the same shape where everything outside a central band in each innermost matrix is set to zero.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func bandPart(
    lowerBandCount: Int,
    upperBandCount: Int
) -> MLTensor
```

## Parameters 

`lowerBandCount`  

The number of diagonals in the lower triangle to keep. If `-1`, keep the entire lower triangle.

`upperBandCount`  

The number of diagonals in the upper triangle to keep. If `-1`, keep the entire upper triangle.

## Return Value

The band part of the tensor.

## Discussion

The framework copies a diagonal band of values from the tensor to the result tensor of the same size. A coordinate `[..., i, j]` is considered in band if

```
```

Values outside of the band are set to `0`.

For example:

```
let t = Tensor([
    [ 5,  1,  2, 3],
    [-1,  5,  1, 2],
    [-2, -1,  5, 1],
    [-3, -2, -1, 5]
], scalarType: Float.self)

t.bandPart(lowerBandCount: 0, upperBandCount: 0)
// [[ 5,  0,  0, 0]
//  [ 0,  5,  0, 0]
//  [ 0,  0,  5, 0]
//  [ 0,  0,  0, 5]]

t.bandPart(lowerBandCount: 0, upperBandCount: -1)
// [[ 5,  1,  2, 3]
//  [ 0,  5,  1, 2]
//  [ 0,  0,  5, 1]
//  [ 0,  0,  0, 5]]

t.bandPart(lowerBandCount: -1, upperBandCount: 0)
// [[ 5,  0,  0, 0]
//  [-1,  5,  0, 0]
//  [-2, -1,  5, 0]
//  [-3, -2, -1, 5]]
```

