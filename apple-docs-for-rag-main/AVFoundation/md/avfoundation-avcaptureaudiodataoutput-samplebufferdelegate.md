

- AVFoundation
- AVCaptureAudioDataOutput
-  sampleBufferDelegate 

Instance Property

# sampleBufferDelegate

The capture object’s delegate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var sampleBufferDelegate: (any AVCaptureAudioDataOutputSampleBufferDelegate)? { get }
```

## Discussion

You use the delegate to manage incoming data.

## See Also

### Receiving Captured Audio Data

func setSampleBufferDelegate((any AVCaptureAudioDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the delegate that will accept captured buffers and the dispatch queue on which the delegate will be called.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which delegate callbacks are invoked

protocol AVCaptureAudioDataOutputSampleBufferDelegate

Methods for receiving audio sample data from an audio capture.

