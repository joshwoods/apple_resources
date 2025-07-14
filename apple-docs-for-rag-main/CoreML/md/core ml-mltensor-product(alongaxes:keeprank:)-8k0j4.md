

- Core ML
- MLTensor
-  product(alongAxes:keepRank:) 

Instance Method

# product(alongAxes:keepRank:)

Returns the product along the specified axes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func product(
    alongAxes axes: [Int],
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
let y = x.product(alongAxes: [0], keepRank: true)
y.shape // is [1, 2]
await y.shapedArray(of: Float.self) // is [48.0 105.0]
```

