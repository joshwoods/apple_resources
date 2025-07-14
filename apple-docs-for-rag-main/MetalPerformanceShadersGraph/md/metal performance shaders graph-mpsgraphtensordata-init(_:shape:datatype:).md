

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(\_:shape:dataType:) 

Initializer

# init(\_:shape:dataType:)

Initializes an tensor data with a metal buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    _ buffer: any MTLBuffer,
    shape: [NSNumber],
    dataType: MPSDataType
)
```

## Parameters 

`buffer`  

MTLBuffer to be used within the MPSGraphTensorData

`shape`  

Shape of the output tensor

`dataType`  

dataType of the placeholder tensor

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

## Discussion

The device of the MTLBuffer will be used to get the MPSDevice for this MPSGraphTensorData.

