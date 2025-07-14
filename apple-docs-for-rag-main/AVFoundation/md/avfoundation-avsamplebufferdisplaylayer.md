

- AVFoundation
-  AVSampleBufferDisplayLayer 

Class

# AVSampleBufferDisplayLayer

An object that displays compressed or uncompressed video frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
class AVSampleBufferDisplayLayer
```

## Topics

### Accessing the video renderer

var sampleBufferRenderer: AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

### Configuring the layer

var isReadyForDisplay: Bool

A Boolean value that indicates whether the first video frame is ready for display.

var controlTimebase: CMTimebase?

A timebase that determines how the layer interprets timestamps.

var videoGravity: AVLayerVideoGravity

A value that indicates how the layer displays video within its bounds.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

### Protecting content

var preventsCapture: Bool

A Boolean value that indicates whether the layer protects against screen capture.

var isOutputObscuredDueToInsufficientExternalProtection: Bool

A Boolean value that indicates whether the system obscures decoded output due to insufficient external protection on the current device.

### Preventing backgrounding

var preventsDisplaySleepDuringVideoPlayback: Bool

A Boolean value that indicates whether the layer prevents the system from sleeping during video playback.

var preventsAutomaticBackgroundingDuringVideoPlayback: Bool

A Boolean value that indicates whether video playback prevents the system from automatically backgrounding an app.

### Handling errors

static let AVSampleBufferDisplayLayerFailedToDecode: NSNotification.Name

A notification the system posts when a sample buffer display layer fails to decode.

let AVSampleBufferDisplayLayerFailedToDecodeNotificationErrorKey: String

The key for the corresponding error.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- CALayer

### Conforms To

- AVQueuedSampleBufferRendering
- CAMediaTiming
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Presentation

protocol AVQueuedSampleBufferRendering

Methods you can implement to enqueue sample buffers for presentation.

class AVSampleBufferRenderSynchronizer

An object used to synchronize multiple queued sample buffers to a single timeline.

class AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

class AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

