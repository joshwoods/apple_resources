

- Core ML
- MLTensor
-  max(keepRank:) 

Instance Method

# max(keepRank:)

Returns the maximum value in the array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func max(keepRank: Bool = false) -> MLTensor
```

## Parameters 

`keepRank`  

A Boolean indicating whether to keep the reduced axes or not. The default value is `false`.

## Return Value

The reduced tensor.

## Discussion

```
let x = MLTensor(shape: [3, 2], scalars: [2, 3, 4, 5, 6, 7], scalarType: Float.self)
let y = x.max()
y.shape // is []
await y.shapedArray(of: Float.self) // is [7.0]
```

