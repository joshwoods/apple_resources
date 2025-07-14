

- AVFoundation
- Sample buffer playback
- AVSampleBufferDisplayLayer
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

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

var hasSufficientMediaDataForReliablePlaybackStart: Bool

A Boolean value that indicates whether the enqueued media data meets the renderer’s preroll level.

Deprecated

### Flushing Sample Buffers

func flush()

Instructs the layer to discard any enqueued sample buffers that are pending.

Deprecated

func flushAndRemoveImage()

Instructs the layer to discard pending enqueued sample buffers and remove any currently displayed image.

Deprecated

### Configuring the Timebase

var timebase: CMTimebase

The renderer’s timebase, which determines how the layer interprets time stamps.

Deprecated

### Enqueuing the Sample Buffer

func enqueue(CMSampleBuffer)

Sends a sample buffer for display.

Deprecated

### Getting Display Layer Settings

var status: AVQueuedSampleBufferRenderingStatus

The ability of the display layer to be used for enqueuing sample buffers.

Deprecated

enum AVQueuedSampleBufferRenderingStatus

The statuses for sample buffer rendering.

### Handling Errors

var error: (any Error)?

The error that caused the failure.

Deprecated

