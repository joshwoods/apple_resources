

- AVFoundation
- AVSampleBufferDisplayLayer
-  isReadyForMoreMediaData Deprecated

Instance Property

# isReadyForMoreMediaData

A Boolean value that indicates the readiness of the layer to accept more sample buffers.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var isReadyForMoreMediaData: Bool { get }
```

Deprecated

Use sampleBufferRenderer's readyForMoreMediaData instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use isReadyForMoreMediaData on the sampleBufferRenderer instead.

`AVSampleBufferDisplayLayer` keeps track of the occupancy levels of its internal queues for the benefit of clients that enqueue sample buffers from non-real-time sources — that is, clients that can supply sample buffers faster than they are consumed and need to decide when to hold back buffers.

Clients enqueueing sample buffers from non-real-time sources may hold off from generating or obtaining more sample buffers to enqueue when the value of `readyForMoreMediaData` is false.

It is safe to call enqueue(_:) when isReadyForMoreMediaData is false, but enqueing more sample buffers than are required for timely rendering by the receiver is highly discouraged.

To help with control of the non-real-time supply of sample buffers, such clients should use requestMediaDataWhenReady(on:using:) in order to specify a block that the layer should invoke whenever it’s ready for sample buffers to be appended.

The value of `readyForMoreMediaData` will often change from false to true asynchronously, as previously supplied sample buffers are decoded and displayed.

Important

This property does not support key-value observing.

## See Also

### Initiating Media Data Requests

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Instructs the target to invoke a client-supplied block repeatedly, at its convenience, in order to gather sample buffers for display.

Deprecated

var requiresFlushToResumeDecoding: Bool

A Boolean value that indicates whether the layer needs to flush its state to continue decoding frames.

Deprecated

func stopRequestingMediaData()

Cancels any current media data request.

Deprecated

var hasSufficientMediaDataForReliablePlaybackStart: Bool

A Boolean value that indicates whether the enqueued media data meets the renderer’s preroll level.

Deprecated

