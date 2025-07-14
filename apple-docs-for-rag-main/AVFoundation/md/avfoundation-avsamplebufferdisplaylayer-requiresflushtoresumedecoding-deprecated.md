

- AVFoundation
- AVSampleBufferDisplayLayer
-  requiresFlushToResumeDecoding Deprecated

Instance Property

# requiresFlushToResumeDecoding

A Boolean value that indicates whether the layer needs to flush its state to continue decoding frames.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var requiresFlushToResumeDecoding: Bool { get }
```

Deprecated

Use sampleBufferRenderer's requiresFlushToResumeDecoding instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use requiresFlushToResumeDecoding on the sampleBufferRenderer instead.

When an app enters a state where use of video decoder resources isn’t permissible, the value of this property changes to true and the display layer’s status changes to a AVQueuedSampleBufferRenderingStatus.failed state.

To resume rendering sample buffers using the display layer after this property’s value is true, apps must first reset the display layer’s status to AVQueuedSampleBufferRenderingStatus.unknown, which you do by calling the layer’s flush() method.

This property isn’t key-value observable. Instead, observe changes to this property value by observing notifications of type AVSampleBufferDisplayLayerRequiresFlushToResumeDecodingDidChangeNotification.

## See Also

### Initiating Media Data Requests

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Instructs the target to invoke a client-supplied block repeatedly, at its convenience, in order to gather sample buffers for display.

Deprecated

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the layer to accept more sample buffers.

Deprecated

func stopRequestingMediaData()

Cancels any current media data request.

Deprecated

var hasSufficientMediaDataForReliablePlaybackStart: Bool

A Boolean value that indicates whether the enqueued media data meets the renderer’s preroll level.

Deprecated

