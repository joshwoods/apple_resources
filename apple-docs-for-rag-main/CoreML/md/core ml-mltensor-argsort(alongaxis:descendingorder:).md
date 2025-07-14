

- Core ML
- MLTensor
-  argsort(alongAxis:descendingOrder:) 

Instance Method

# argsort(alongAxis:descendingOrder:)

Returns the indices (or arguments) of a tensor that give its sorted order along the specified axis.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func argsort(
    alongAxis axis: Int = -1,
    descendingOrder: Bool = false
) -> MLTensor
```

## Parameters 

`axis`  

The axis along which to sort. The default is `-1`, which sorts the last axis.

`descendingOrder`  

A Boolean value that determines the sort order. The default is `false` which sorts from largest to least.

## Return Value

A `Int32` tensor of sorted indices.

## Discussion

For example:

```
let x = MLTensor([1.0, 3.0, 2.0])
let y = x.argSort()
await y.shapedArray(of: Int32.self) // is [0, 2, 1]
```

