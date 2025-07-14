

- AVFoundation
- AVSampleBufferDisplayLayer
-  stopRequestingMediaData() Deprecated

Instance Method

# stopRequestingMediaData()

Cancels any current media data request.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func stopRequestingMediaData()
```

Deprecated

Use sampleBufferRenderer's stopRequestingMediaData instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use stopRequestingMediaData() on the sampleBufferRenderer instead.

This method cancels any current requestMediaDataWhenReady(on:using:) call. Each invocation of requestMediaDataWhenReady(on:using:) must be balanced by a call to this method.

This method may be called from within the requestMediaDataWhenReady(on:using:) method’s block or from outside the block.

## See Also

### Initiating Media Data Requests

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Instructs the target to invoke a client-supplied block repeatedly, at its convenience, in order to gather sample buffers for display.

Deprecated

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the layer to accept more sample buffers.

Deprecated

var requiresFlushToResumeDecoding: Bool

A Boolean value that indicates whether the layer needs to flush its state to continue decoding frames.

Deprecated

var hasSufficientMediaDataForReliablePlaybackStart: Bool

A Boolean value that indicates whether the enqueued media data meets the renderer’s preroll level.

Deprecated

