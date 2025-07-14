

- AVFoundation
-  AVQueuedSampleBufferRendering 

Protocol

# AVQueuedSampleBufferRendering

Methods you can implement to enqueue sample buffers for presentation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol AVQueuedSampleBufferRendering : NSObjectProtocol
```

## Overview

AVSampleBufferDisplayLayer and AVSampleBufferAudioRenderer conform to this protocol. When used in conjunction with an AVSampleBufferRenderSynchronizer, an object conforming to `AVQueuedSampleBufferRendering` can only be attached to a single synchronizer.

## Topics

### Requesting Media

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the receiver is able to accept more sample buffers.

**Required**

func enqueue(CMSampleBuffer)

Sends a sample buffer to the queue for rendering.

**Required**

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the target to invoke a client-supplied block in order to gather sample buffers for playback.

**Required**

func stopRequestingMediaData()

Cancels any current requestMediaDataWhenReady(on:using:) call.

**Required**

### Determining Playback Readiness

var hasSufficientMediaDataForReliablePlaybackStart: Bool

A Boolean value that indicates whether the enqued media meets the required preroll level for reliable playback.

**Required**

### Clearing Queued Sample Buffers

func flush()

Discards all pending enqueued sample buffers.

**Required**

### Indentifying the Timebase

var timebase: CMTimebase

The timebase for a renderer.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- AVSampleBufferAudioRenderer
- AVSampleBufferDisplayLayer
- AVSampleBufferVideoRenderer

## See Also

### Presentation

class AVSampleBufferRenderSynchronizer

An object used to synchronize multiple queued sample buffers to a single timeline.

class AVSampleBufferDisplayLayer

An object that displays compressed or uncompressed video frames.

class AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

class AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

