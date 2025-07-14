

- AVFoundation
- AVSampleBufferDisplayLayer
-  requestMediaDataWhenReady(on:using:) Deprecated

Instance Method

# requestMediaDataWhenReady(on:using:)

Instructs the target to invoke a client-supplied block repeatedly, at its convenience, in order to gather sample buffers for display.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func requestMediaDataWhenReady(
    on queue: dispatch_queue_t,
    using block: @escaping () -> Void
)
```

Deprecated

Use sampleBufferRenderer's requestMediaDataWhenReadyOnQueue:usingBlock: instead

## Parameters 

`queue`  

The dispatch queue.

`block`  

The block that provides media data.

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use requestMediaDataWhenReady(on:using:) on the sampleBufferRenderer instead.

The block is expected to call the enqueue(_:) in order to provide media data for decompression (if necessary) and rendering while the isReadyForMoreMediaData property remains true, or until it can provide no additional media. When the layer has decoded enough media data that it is ready for additional media data, it will invoke the block again.

By allowing the display layer to determine when to invoke the block, the implementation of incremental I/O operations is simplified when supplying synchronized media data during rendering.

If this function is called multiple times, only the last call is effective.

You invoke the stopRequestingMediaData() method to cancel this request.

Each call to `requestMediaDataWhenReadyOnQueue:usingBlock:` must be balanced with a corresponding call to stopRequestingMediaData().

Releasing the receiver instance without a call to stopRequestingMediaData() will result in undefined behavior.

## See Also

### Initiating Media Data Requests

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the layer to accept more sample buffers.

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

