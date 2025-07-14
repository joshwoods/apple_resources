

- AVFoundation
- AVCaptureSynchronizedDepthData
-  depthDataWasDropped 

Instance Property

# depthDataWasDropped

A Boolean value indicating whether depth data was discarded between capture and processing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var depthDataWasDropped: Bool { get }
```

## Discussion

If this value is true, depth data was captured for this synchronization point but could not be delivered. This situation differs from that where no depth data capture for the synchronization timestamp occurs. In that case, there is no AVCaptureSynchronizedDepthData object present in the AVCaptureSynchronizedDataCollection object delivered to your delegate method.

## See Also

### Handling Dropped Data

var droppedReason: AVCaptureOutput.DataDroppedReason

A value indicating why the capture output failed to deliver depth data, if applicable.

