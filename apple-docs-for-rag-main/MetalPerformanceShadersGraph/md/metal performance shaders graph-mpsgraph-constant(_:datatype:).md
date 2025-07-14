

- Metal Performance Shaders Graph
- MPSGraph
-  constant(\_:dataType:) 

Instance Method

# constant(\_:dataType:)

Creates a constant operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func constant(
    _ scalar: Double,
    dataType: MPSDataType
) -> MPSGraphTensor
```

## Parameters 

`scalar`  

The scalar value to fill the entire tensor values with.

`dataType`  

The dataType of the constant tensor.

## Return Value

A valid MPSGraphTensor object.

