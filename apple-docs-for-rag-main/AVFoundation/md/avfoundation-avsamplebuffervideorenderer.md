

- AVFoundation
-  AVSampleBufferVideoRenderer 

Class

# AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class AVSampleBufferVideoRenderer
```

## Topics

### Flushing the renderer

var requiresFlushToResumeDecoding: Bool

A Boolean value that Indicates whether the renderer requires flushing to continue decoding frames.

class let requiresFlushToResumeDecodingDidChangeNotification: NSNotification.Name

A notification that indicates that the video renderer requires flushing to continue rendering sample buffers.

func flush(removingDisplayedImage: Bool, completionHandler: (() -> Void)?)

Tells the video renderer to discard pending enqueued sample buffers.

### Inspecting the status

var status: AVQueuedSampleBufferRenderingStatus

A status value that indicates whether this object can enqueue and render sample buffers.

var error: (any Error)?

An object the describes the error that caused the rendering failure.

### Handling decode failures

class let didFailToDecodeNotification: NSNotification.Name

A notification that indicates the video renderer fails to decode a sample buffer.

class let didFailToDecodeNotificationErrorKey: String

A key to retrieve an error object that provides the details of the failure.

### Instance Properties

var presentationTimeExpectation: AVSampleBufferVideoRenderer.PresentationTimeExpectation

### Instance Methods

func displayedPixelBuffer() -> CVPixelBuffer?

func loadVideoPerformanceMetrics(completionHandler: (AVVideoPerformanceMetrics?) -> Void)

### Enumerations

enum PresentationTimeExpectation

## Relationships

### Inherits From

- NSObject

### Conforms To

- AVQueuedSampleBufferRendering
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Presentation

protocol AVQueuedSampleBufferRendering

Methods you can implement to enqueue sample buffers for presentation.

class AVSampleBufferRenderSynchronizer

An object used to synchronize multiple queued sample buffers to a single timeline.

class AVSampleBufferDisplayLayer

An object that displays compressed or uncompressed video frames.

class AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

