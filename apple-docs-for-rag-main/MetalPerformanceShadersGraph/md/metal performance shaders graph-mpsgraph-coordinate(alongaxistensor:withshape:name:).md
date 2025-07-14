

- Metal Performance Shaders Graph
- MPSGraph
-  coordinate(alongAxisTensor:withShape:name:) 

Instance Method

# coordinate(alongAxisTensor:withShape:name:)

Creates a get-coordindate operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func coordinate(
    alongAxisTensor axisTensor: MPSGraphTensor,
    withShape shape: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axisTensor`  

A Scalar tensor of type `MPSDataTypeInt32`, that specifies the coordinate axis an element’s value is set to. Negative values wrap around.

`shape`  

The shape of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

See coordinate(alongAxis:withShape:name:).

