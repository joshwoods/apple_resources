

- AVFoundation
-  AVSampleBufferRenderSynchronizer 

Class

# AVSampleBufferRenderSynchronizer

An object used to synchronize multiple queued sample buffers to a single timeline.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class AVSampleBufferRenderSynchronizer
```

## Mentioned in 

Implementing flexible enhanced buffering for your content

Supporting AirPlay in your app

## Overview

This class synchronizes multiple objects that conform to AVQueuedSampleBufferRendering to a single timeline.

## Topics

### Managing Renderers

var renderers: [any AVQueuedSampleBufferRendering]

An array of queued sample buffer renderers currently attached to the synchronizer.

func addRenderer(any AVQueuedSampleBufferRendering)

Adds a renderer to the list of renderers under the synchronizer’s control.

func removeRenderer(any AVQueuedSampleBufferRendering, at: CMTime, completionHandler: ((Bool) -> Void)?)

Removes a renderer from the synchronizer.

### Accessing Time Information

func currentTime() -> CMTime

Returns the current time of the synchronizer.

var timebase: CMTimebase

The synchronizer’s rendering timebase which determines how it interprets timestamps.

var rate: Float

The current playback rate.

func setRate(Float, time: CMTime)

Sets the renderer’s time and rate.

func setRate(Float, time: CMTime, atHostTime: CMTime)

Sets the playback rate and the relationship between the current time and host time.

class let rateDidChangeNotification: NSNotification.Name

The synchronizer’s rendering rate changed.

var delaysRateChangeUntilHasSufficientMediaData: Bool

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

### Observing Time

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests invocation of a block during rendering at specified time intervals.

func addBoundaryTimeObserver(forTimes: [NSValue], queue: dispatch_queue_t?, using: () -> Void) -> Any

Requests invocation of a block when specified times are traversed during normal rendering.

func removeTimeObserver(Any)

Cancels the specified time observer.

## Relationships

### Inherits From

- NSObject

### Conforms To

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

class AVSampleBufferDisplayLayer

An object that displays compressed or uncompressed video frames.

class AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

class AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

