

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(\_:) 

Initializer

# init(\_:)

Initializes an MPSGraphTensorData with an MPS ndarray.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(_ ndarray: MPSNDArray)
```

## Parameters 

`ndarray`  

MPSNDArray to be used within the MPSGraphTensorData.

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

## Discussion

The device of the MPSNDArray will be used to get the MPSDevice for this MPSGraphTensorData.

