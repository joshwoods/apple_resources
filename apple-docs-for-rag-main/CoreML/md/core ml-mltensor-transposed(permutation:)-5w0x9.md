

- Core ML
- MLTensor
-  transposed(permutation:) 

Instance Method

# transposed(permutation:)

Permutes the dimensions of the tensor in the specified order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func transposed(permutation: Int...) -> MLTensor
```

## Parameters 

`permutation`  

An array of integers defining the permutation, must be of length `rank` and define a valid permutation.

## Return Value

A permuted tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [1, 2, 3], scalars: [1, 2, 3, 4, 5, 6], scalarType: Float.self)
let y = x.transposed(1, 0, 2)
y.shape // is [2, 1, 3]
```

