

- AVFoundation
- AVCaptureSynchronizedSampleBufferData
-  droppedReason 

Instance Property

# droppedReason

A value indicating why the capture output failed to deliver sample buffers, if applicable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var droppedReason: AVCaptureOutput.DataDroppedReason { get }
```

## See Also

### Handling Dropped Data

var sampleBufferWasDropped: Bool

A Boolean value indicating whether sample buffers were discarded between capture and processing.

