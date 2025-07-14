

- Core ML
- MLTensor
-  min(alongAxes:keepRank:) 

Instance Method

# min(alongAxes:keepRank:)

Returns the minimum values along the specified axes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func min(
    alongAxes axes: Int...,
    keepRank: Bool = false
) -> MLTensor
```

## Parameters 

`axes`  

The axes to reduce.

`keepRank`  

A Boolean indicating whether to keep the reduced axes or not. The default value is `false`.

## Return Value

The reduced tensor.

## Discussion

```
let x = MLTensor(shape: [3, 2], scalars: [2, 3, 4, 5, 6, 7], scalarType: Float.self)
let y = x.min(alongAxes: 0)
y.shape // is [1, 2]
await y.shapedArray(of: Float.self) // is [2.0 3.0]
```

