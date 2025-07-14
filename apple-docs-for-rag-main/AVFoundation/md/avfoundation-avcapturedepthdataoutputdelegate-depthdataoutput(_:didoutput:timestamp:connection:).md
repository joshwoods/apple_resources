

- AVFoundation
- AVCaptureDepthDataOutputDelegate
-  depthDataOutput(\_:didOutput:timestamp:connection:) 

Instance Method

# depthDataOutput(\_:didOutput:timestamp:connection:)

Provides newly captured depth data to the delegate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func depthDataOutput(
    _ output: AVCaptureDepthDataOutput,
    didOutput depthData: AVDepthData,
    timestamp: CMTime,
    connection: AVCaptureConnection
)
```

## Parameters 

`output`  

The depth data output providing data.

`depthData`  

A depth data object containing the captured per-pixel depth data.

`timestamp`  

The time at which the data was captured.

`connection`  

The capture connection through which the data was captured.

## Discussion

The depth data output calls this method whenever it captures and outputs a new depth data object. This method is called on the dispatch queue specified by the output’s delegateCallbackQueue property, and can be called frequently. Your implementation must process the depth data quickly in order to prevent dropped depth data.

To maintain optimal performance, the capture pipeline may allocate AVDepthData pixel buffer maps from a finite memory pool. If you hold on to any AVDepthData objects for too long, capture inputs cannot copy new depth data into memory, resulting in dropped depth data. If your application is causing depth data drops by holding on to provided depth data objects for too long, consider copying the pixel buffer map data into a new pixel buffer so that the AVDepthData backing memory can be reused more quickly.

## See Also

### Receiving Depth Data

func depthDataOutput(AVCaptureDepthDataOutput, didDrop: AVDepthData, timestamp: CMTime, connection: AVCaptureConnection, reason: AVCaptureOutput.DataDroppedReason)

Informs the delegate that captured depth data was not processed.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

