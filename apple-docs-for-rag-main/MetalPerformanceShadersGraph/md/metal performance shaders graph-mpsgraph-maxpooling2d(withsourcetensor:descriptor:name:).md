

- Metal Performance Shaders Graph
- MPSGraph
-  maxPooling2D(withSourceTensor:descriptor:name:) 

Instance Method

# maxPooling2D(withSourceTensor:descriptor:name:)

Creates a 2D max-pooling operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func maxPooling2D(
    withSourceTensor source: MPSGraphTensor,
    descriptor: MPSGraphPooling2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

A 2D Image source as tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`descriptor`  

A pooling operation descriptor that specifies pooling window sizes, strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

