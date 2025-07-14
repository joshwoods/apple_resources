

- Metal Performance Shaders Graph
- MPSGraph
-  scaledDotProductAttention(query:key:value:scale:name:) 

Instance Method

# scaledDotProductAttention(query:key:value:scale:name:)

Creates a scaled dot product attention (SDPA) operation (without a mask) and returns the result tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func scaledDotProductAttention(
    query queryTensor: MPSGraphTensor,
    key keyTensor: MPSGraphTensor,
    value valueTensor: MPSGraphTensor,
    scale: Float,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`queryTensor`  

A tensor that represents the query projection.

`keyTensor`  

A tensor that represents the key projection.

`valueTensor`  

A tensor that represents the value projection.

`scale`  

A scale that is applied on the result of query and value matrix multiply.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

