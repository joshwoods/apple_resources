

- AVFoundation
- AVCaptureSynchronizedSampleBufferData
-  sampleBufferWasDropped 

Instance Property

# sampleBufferWasDropped

A Boolean value indicating whether sample buffers were discarded between capture and processing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sampleBufferWasDropped: Bool { get }
```

## Discussion

If this value is true, sample buffers were captured for this synchronization point but could not be delivered. This situation differs from that where no sample buffer capture for the synchronization timestamp occurs. In that case, there is no AVCaptureSynchronizedSampleBufferData object present in the AVCaptureSynchronizedDataCollection object delivered to your delegate method.

## See Also

### Handling Dropped Data

var droppedReason: AVCaptureOutput.DataDroppedReason

A value indicating why the capture output failed to deliver sample buffers, if applicable.

