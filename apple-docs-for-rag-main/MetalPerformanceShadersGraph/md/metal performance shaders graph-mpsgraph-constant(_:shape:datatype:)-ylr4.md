

- Metal Performance Shaders Graph
- MPSGraph
-  constant(\_:shape:dataType:) 

Instance Method

# constant(\_:shape:dataType:)

Creates a constant op with a given shape and data, and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func constant(
    _ data: Data,
    shape: [NSNumber],
    dataType: MPSDataType
) -> MPSGraphTensor
```

## Parameters 

`data`  

The data for the tensor. The number of bytes should be sizeof(dataType)numberOfElements.

`shape`  

The shape of the output tensor. This has to be statically shaped.

`dataType`  

The dataType of theconstant tensor.

## Return Value

A valid MPSGraphTensor object.

