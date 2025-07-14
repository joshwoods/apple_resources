

- Metal Performance Shaders Graph
- MPSGraph
-  imToCol(\_:descriptor:name:) 

Instance Method

# imToCol(\_:descriptor:name:)

Creates an imToCol operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func imToCol(
    _ source: MPSGraphTensor,
    descriptor: MPSGraphImToColOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

The tensor containing the source data. Must be of rank 4. The layout is defined by `descriptor.dataLayout`.

`descriptor`  

The descriptor object that specifies the parameters of the operation.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

