

- Metal Performance Shaders Graph
- MPSGraph
-  placeholder(shape:name:) 

Instance Method

# placeholder(shape:name:)

Creates a placeholder operation and returns the result tensor with the dataType of the placeholder tensor set to 32 bit float.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func placeholder(
    shape: [NSNumber]?,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`shape`  

The shape of the output tensor. A nil shape will result in an unranked tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

