

- Metal Performance Shaders Graph
- MPSGraph
-  variable(with:shape:dataType:name:) 

Instance Method

# variable(with:shape:dataType:name:)

Creates a variable operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func variable(
    with data: Data,
    shape: [NSNumber],
    dataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`data`  

The data for the tensor. The number of bytes should be sizeof(dataType)numberOfElements.

`shape`  

The shape of the output tensor. This has to be statically shaped.

`dataType`  

The dataType of the constant tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

