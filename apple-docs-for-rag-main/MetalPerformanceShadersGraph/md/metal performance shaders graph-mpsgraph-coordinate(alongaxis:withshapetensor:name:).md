

- Metal Performance Shaders Graph
- MPSGraph
-  coordinate(alongAxis:withShapeTensor:name:) 

Instance Method

# coordinate(alongAxis:withShapeTensor:name:)

Creates a get-coordindate operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func coordinate(
    alongAxis axis: Int,
    withShapeTensor shapeTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axis`  

The coordinate axis an element’s value is set to. Negative values wrap around.

`shapeTensor`  

A rank-1 tensor of type `MPSDataTypeInt32` or `MPSDataTypeInt64` that defines the shape of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

See coordinate(alongAxis:withShape:name:).

