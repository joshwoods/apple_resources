

- AVFoundation
- AVCaptureVideoDataOutput
-  sampleBufferDelegate 

Instance Property

# sampleBufferDelegate

The capture object’s delegate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var sampleBufferDelegate: (any AVCaptureVideoDataOutputSampleBufferDelegate)? { get }
```

## Discussion

The delegate receives sample buffers after they are captured.

You set the delegate using setSampleBufferDelegate(_:queue:).

## See Also

### Receiving Captured Video Data

func setSampleBufferDelegate((any AVCaptureVideoDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the sample buffer delegate and the queue for invoking callbacks.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which the system invokes delegate callbacks.

protocol AVCaptureVideoDataOutputSampleBufferDelegate

Methods for receiving sample buffers from, and monitoring the status of, a video data output.

