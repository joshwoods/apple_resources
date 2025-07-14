

- Core ML
- MLTensor
-  replacing(with:where:) 

Instance Method

# replacing(with:where:)

Returns a new tensor replacing the value of `other` with the corresponding element in `self` where the associated element in `mask` is `true`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func replacing(
    with replacement: some MLTensorScalar,
    where mask: MLTensor
) -> MLTensor
```

## Parameters 

`replacement`  

The replacement value where `mask` is `true`.

`mask`  

The Boolean mask that determines whether the corresponding element / row should be taken from `self` (if the element in `mask` is `false`) or `other` (if `true`).

## Return Value

A new tensor of the same shape and type as `self`.

## Discussion

For example:

```
let x = MLTensor([1, 2, 3], scalarType: Float.self)
let mask = MLTensor([false, true, false])
let z = x.replacing(with: 5, where: mask)
await z.shapedArray(of: Float.self) // is [1, 5, 3]
```

