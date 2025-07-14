

- Core ML
- MLTensor
-  mean(keepRank:) 

Instance Method

# mean(keepRank:)

Returns the mean along all axes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func mean(keepRank: Bool = false) -> MLTensor
```

## Parameters 

`keepRank`  

A Boolean indicating whether to keep the reduced axes or not. The default value is `false`.

## Return Value

The reduced tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [3, 2], scalars: [2, 3, 4, 5, 6, 7], scalarType: Float.self)
let y = x.mean()
y.shape // is []
await y.shapedArray(of: Float.self) // is [4.5]
```

