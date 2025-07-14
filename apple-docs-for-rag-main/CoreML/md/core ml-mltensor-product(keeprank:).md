

- Core ML
- MLTensor
-  product(keepRank:) 

Instance Method

# product(keepRank:)

Returns the product along all axes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func product(keepRank: Bool = false) -> MLTensor
```

## Parameters 

`keepRank`  

A Boolean indicating whether to keep the reduced axes or not. The default value is `false`.

## Return Value

The reduced tensor.

## Discussion

```
let x = MLTensor(shape: [3, 2], scalars: [2, 3, 4, 5, 6, 7], scalarType: Float.self)
let y = x.product()
y.shape // is []
await y.shapedArray(of: Float.self) // is [5040.0]
```

