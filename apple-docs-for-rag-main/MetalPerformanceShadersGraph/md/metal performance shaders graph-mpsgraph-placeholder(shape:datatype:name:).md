

- Metal Performance Shaders Graph
- MPSGraph
-  placeholder(shape:dataType:name:) 

Instance Method

# placeholder(shape:dataType:name:)

Creates a placeholder operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func placeholder(
    shape: [NSNumber]?,
    dataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`shape`  

The shape of the output tensor. A nil shape will result in an unranked tensor.

`dataType`  

The dataType of the placeholder tensor.

`name`  

The name for the placeholder operation.

## Return Value

A valid MPSGraphTensor object.

