

- AVFoundation
- AVCaptureAudioDataOutput
-  setSampleBufferDelegate(\_:queue:) 

Instance Method

# setSampleBufferDelegate(\_:queue:)

Sets the delegate that will accept captured buffers and the dispatch queue on which the delegate will be called.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func setSampleBufferDelegate(
    _ sampleBufferDelegate: (any AVCaptureAudioDataOutputSampleBufferDelegate)?,
    queue sampleBufferCallbackQueue: dispatch_queue_t?
)
```

## Parameters 

`sampleBufferDelegate`  

An object conforming to the AVCaptureAudioDataOutputSampleBufferDelegate protocol that will receive sample buffers after they are captured.

`sampleBufferCallbackQueue`  

You must pass a serial dispatch to guarantee that audio samples will be delivered in order.

The value may not be `NULL`, except when setting the `sampleBufferDelegate` to `nil`.

## Discussion

When a new audio sample buffer is captured it is vended to the sample buffer delegate using the captureOutput(_:didOutput:from:) delegate method. All delegate methods are called on the specified dispatch queue.

If the queue is blocked when new samples are captured, those samples will be automatically dropped when they become sufficiently late. This allows you to process existing samples on the same queue without having to manage the potential memory usage increases that would otherwise occur when that processing is unable to keep up with the rate of incoming samples.

If you need to minimize the chances of samples being dropped, you should specify a queue on which a sufficiently small amount of processing is being done outside of receiving sample buffers. When migrating extra processing to another queue, you are responsible for ensuring that memory usage does not grow without bound from samples that have not been processed.

### Special Considerations

This method uses dispatch_retain and dispatch_release to manage the queue.

## See Also

### Receiving Captured Audio Data

var sampleBufferDelegate: (any AVCaptureAudioDataOutputSampleBufferDelegate)?

The capture object’s delegate.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which delegate callbacks are invoked

protocol AVCaptureAudioDataOutputSampleBufferDelegate

Methods for receiving audio sample data from an audio capture.

