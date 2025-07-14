

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(\_:rank:) 

Initializer

# init(\_:rank:)

Initializes a tensor data with an MPS vector enforcing rank of the result.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    _ vector: MPSVector,
    rank: Int
)
```

## Parameters 

`vector`  

MPSVector to be used within the MPSGraphTensorData

`rank`  

The rank of the resulting TensorData tensor. NOTE: must be within { 1, … ,16 }.

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

## Discussion

The device of the MPSVector will be used to get the MPSDevice for this MPSGraphTensorData.

