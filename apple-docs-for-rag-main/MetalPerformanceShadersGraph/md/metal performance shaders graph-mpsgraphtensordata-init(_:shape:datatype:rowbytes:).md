

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(\_:shape:dataType:rowBytes:) 

Initializer

# init(\_:shape:dataType:rowBytes:)

Initializes an tensor data with a metal buffer.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
init(
    _ buffer: any MTLBuffer,
    shape: [NSNumber],
    dataType: MPSDataType,
    rowBytes: Int
)
```

## Parameters 

`buffer`  

MTLBuffer to be used within the MPSGraphTensorData

`shape`  

Shape of the output tensor

`dataType`  

dataType of the placeholder tensor

`rowBytes`  

rowBytes for the fastest moving dimension, must be larger than or equal to sizeOf(dataType)shape\[rank - 1\] and must be a multiple of sizeOf(dataType)

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

## Discussion

The device of the MTLBuffer will be used to get the MPSDevice for this MPSGraphTensorData.

