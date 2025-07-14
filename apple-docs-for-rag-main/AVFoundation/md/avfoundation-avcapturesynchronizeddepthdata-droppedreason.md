

- AVFoundation
- AVCaptureSynchronizedDepthData
-  droppedReason 

Instance Property

# droppedReason

A value indicating why the capture output failed to deliver depth data, if applicable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var droppedReason: AVCaptureOutput.DataDroppedReason { get }
```

## See Also

### Handling Dropped Data

var depthDataWasDropped: Bool

A Boolean value indicating whether depth data was discarded between capture and processing.

