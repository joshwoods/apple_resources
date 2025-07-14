

- Core ML
- MLTensor
-  tiled(multiples:) 

Instance Method

# tiled(multiples:)

Returns a tensor by replicating its elements multiple times.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func tiled(multiples: [Int]) -> MLTensor
```

## Parameters 

`multiples`  

The multiplier across each dimension. All values must be greater than zero.

## Return Value

The replicated tensor.

## Discussion

The `multiples` argument specifies the multiplier across each dimensions, i.e., the output dimension at index `i` is equal to `shape[i] * multiples[i]`.

For example:

```
let x = MLTensor(shape: [2, 2], scalars: [1, 2, 3, 4], scalarType: Float.self)
let y = x.tiled(multiples: [1, 2])
y.shape // is [2, 4]
```

If `multiples` specifies fewer dimensions than the tensor, then ones are prepended to `multiples` until all the dimensions are specified.

If tensor has fewer dimensions than `multiples`, then the tensor is reshaped by prepending ones to the dimensions until all the dimensions are specified.

