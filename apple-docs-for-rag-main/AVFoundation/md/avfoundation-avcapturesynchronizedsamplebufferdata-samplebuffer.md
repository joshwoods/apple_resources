

- AVFoundation
- AVCaptureSynchronizedSampleBufferData
-  sampleBuffer 

Instance Property

# sampleBuffer

The depth data captured at this synchronization point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sampleBuffer: CMSampleBuffer { get }
```

## Discussion

Note that if the sampleBufferWasDropped property is true, this CMSampleBuffer object does not contain pixel data (instead, it contains only metadata).

This value is equivalent to that provided by the captureOutput(_:didOutput:from:) or captureOutput(_:didDrop:from:) delegate method when using a video data output without a data output synchronizer.

