

- AVFoundation
- AVSampleBufferDisplayLayer
-  hasSufficientMediaDataForReliablePlaybackStart Deprecated

Instance Property

# hasSufficientMediaDataForReliablePlaybackStart

A Boolean value that indicates whether the enqueued media data meets the renderer’s preroll level.

iOS 14.5–18.0DeprecatediPadOS 14.5–18.0DeprecatedMac Catalyst 14.5–18.0DeprecatedmacOS 11.3–15.0DeprecatedtvOS 14.5–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var hasSufficientMediaDataForReliablePlaybackStart: Bool { get }
```

Deprecated

Use sampleBufferRenderer's hasSufficientMediaDataForReliablePlaybackStart instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use hasSufficientMediaDataForReliablePlaybackStart on the sampleBufferRenderer instead.

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

func stopRequestingMediaData()

Cancels any current media data request.

Deprecated

