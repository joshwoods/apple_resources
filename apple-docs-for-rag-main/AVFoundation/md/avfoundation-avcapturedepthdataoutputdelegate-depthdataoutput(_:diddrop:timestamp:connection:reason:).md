

- AVFoundation
- AVCaptureDepthDataOutputDelegate
-  depthDataOutput(\_:didDrop:timestamp:connection:reason:) 

Instance Method

# depthDataOutput(\_:didDrop:timestamp:connection:reason:)

Informs the delegate that captured depth data was not processed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func depthDataOutput(
    _ output: AVCaptureDepthDataOutput,
    didDrop depthData: AVDepthData,
    timestamp: CMTime,
    connection: AVCaptureConnection,
    reason: AVCaptureOutput.DataDroppedReason
)
```

## Parameters 

`output`  

The depth data output providing data.

`depthData`  

A depth data object containing information about the dropped data, such as its data type. Because this depth data was not captured or processed, its depthDataMap property is empty.

`timestamp`  

The time at which the data was captured.

`connection`  

The capture connection through which the data was captured.

`reason`  

The reason depth data was dropped.

## Discussion

The capture output calls this method once for each incident of dropped depth data. The object in the `depthData` parameter is an empty shell, and doesn’t contain a depth data backing pixel buffer.

The capture output calls this method on the dispatch queue specified by its delegateCallbackQueue property. Because this method executes on the same dispatch queue that outputs depth data, your implementation must be efficient to prevent further capture performance problems such as additional drops.

## See Also

### Receiving Depth Data

func depthDataOutput(AVCaptureDepthDataOutput, didOutput: AVDepthData, timestamp: CMTime, connection: AVCaptureConnection)

Provides newly captured depth data to the delegate.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

