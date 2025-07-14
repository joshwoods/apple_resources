

- Metal Performance Shaders Graph
- MPSGraph
-  colToIm(\_:outputShape:descriptor:name:) 

Instance Method

# colToIm(\_:outputShape:descriptor:name:)

Creates a column to image operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func colToIm(
    _ source: MPSGraphTensor,
    outputShape: [NSNumber],
    descriptor: MPSGraphImToColOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

The tensor containing the source data. Must be of rank 4. The layout is defined by `descriptor.dataLayout`.

`outputShape`  

The result tensor shape.

`descriptor`  

The descriptor object that specifies the parameters of the operation.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

