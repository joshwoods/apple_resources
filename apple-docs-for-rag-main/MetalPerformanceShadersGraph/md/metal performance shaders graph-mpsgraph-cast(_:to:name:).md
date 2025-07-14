

- Metal Performance Shaders Graph
- MPSGraph
-  cast(\_:to:name:) 

Instance Method

# cast(\_:to:name:)

Creates a cast operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func cast(
    _ tensor: MPSGraphTensor,
    to type: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`type`  

The datatype to which MPSGraph casts the input.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Returns the input tensor casted to the specied data type.

