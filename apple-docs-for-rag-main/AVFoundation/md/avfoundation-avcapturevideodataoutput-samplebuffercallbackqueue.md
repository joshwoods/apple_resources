

- AVFoundation
- AVCaptureVideoDataOutput
-  sampleBufferCallbackQueue 

Instance Property

# sampleBufferCallbackQueue

The queue on which the system invokes delegate callbacks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var sampleBufferCallbackQueue: dispatch_queue_t? { get }
```

## Discussion

You set the queue using setSampleBufferDelegate(_:queue:).

## See Also

### Receiving Captured Video Data

func setSampleBufferDelegate((any AVCaptureVideoDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the sample buffer delegate and the queue for invoking callbacks.

var sampleBufferDelegate: (any AVCaptureVideoDataOutputSampleBufferDelegate)?

The capture object’s delegate.

protocol AVCaptureVideoDataOutputSampleBufferDelegate

Methods for receiving sample buffers from, and monitoring the status of, a video data output.

