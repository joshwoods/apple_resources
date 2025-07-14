

- AVFoundation
-  AVSampleBufferAudioRenderer 

Class

# AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class AVSampleBufferAudioRenderer
```

## Mentioned in 

Supporting AirPlay in your app

Implementing flexible enhanced buffering for your content

## Overview

You must add an instance of this class to an AVSampleBufferRenderSynchronizer before queuing the first sample buffer.

## Topics

### Determining Rendering Status

var status: AVQueuedSampleBufferRenderingStatus

The status of the audio renderer.

enum AVQueuedSampleBufferRenderingStatus

The statuses for sample buffer rendering.

### Removing Queued Buffers

func flush(fromSourceTime: CMTime, completionHandler: (Bool) -> Void)

Flushes queued sample buffers with presentation time stamps later than or equal to the specified time.

let AVSampleBufferAudioRendererFlushTimeKey: String

The key that indicates the presentation timestamp of the first queued sample that was flushed.

### Configuring Time and Pitch

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm used to manage audio pitch at different rates.

struct AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

### Configuring Audio Spatialization

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the audio renderer supports for spatialization.

### Managing Audio Output

var volume: Float

The current audio volume for the audio renderer.

var isMuted: Bool

A Boolean value that indicates whether audio for the renderer is in a muted state.

var audioOutputDeviceUniqueID: String?

The unique identifier of the output device used to play audio.

### Responding to Errors

var error: (any Error)?

The error that caused the renderer to no longer render sample buffers.

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

class AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

