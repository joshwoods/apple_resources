

- Core ML
- MLTensor
-  any(alongAxes:keepRank:) 

Instance Method

# any(alongAxes:keepRank:)

Computes logical OR on elements across the specified axes of a tensor where the scalar type of the tensor is expected to be Boolean.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func any(
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

The reduced Boolean tensor.

