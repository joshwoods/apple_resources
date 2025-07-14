

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(\_:) 

Initializer

# init(\_:)

Initializes a tensor data with an MPS matrix.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(_ matrix: MPSMatrix)
```

## Parameters 

`matrix`  

MPSMatrix to be used within the MPSGraphTensorData

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

## Discussion

The device of the MPSMatrix will be used to get the MPSDevice for this MPSGraphTensorData.

