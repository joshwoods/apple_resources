

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  init(device:data:shape:dataType:) 

Initializer

# init(device:data:shape:dataType:)

Initializes the tensor data with an `NSData` on a device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    device: MPSGraphDevice,
    data: Data,
    shape: [NSNumber],
    dataType: MPSDataType
)
```

## Parameters 

`device`  

MPSDevice on which the MPSGraphTensorData exists

`data`  

NSData from which to copy the contents

`shape`  

Shape of the output tensor

`dataType`  

dataType of the placeholder tensor

## Return Value

A valid MPSGraphTensorData, or nil if allocation failure.

