

- AVFoundation
-  AVAsynchronousVideoCompositionRequest 

Class

# AVAsynchronousVideoCompositionRequest

An object that contains information a video compositor needs to render an output pixel buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAsynchronousVideoCompositionRequest
```

## Overview

The video compositor must adopt the AVVideoCompositing protocol.

## Topics

### Inspecting the Request

var compositionTime: CMTime

A time for which to compose the frame.

var renderContext: AVVideoCompositionRenderContext

The rendering context of the video composition.

var videoCompositionInstruction: any AVVideoCompositionInstructionProtocol

A video composition instruction that indicates how to compose the frame.

### Accessing Source Data

var sourceTrackIDs: [NSNumber]

The identifiers of tracks that contain source video.

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of tracks that contain source sample data.

func sourceFrame(byTrackID: CMPersistentTrackID) -> CVPixelBuffer?

Returns a source pixel buffer for the track that contains the specified identifier.

func sourceSampleBuffer(byTrackID: CMPersistentTrackID) -> CMSampleBuffer?

Returns a source sample buffer for the track that contains the specified identifier.

func sourceTimedMetadata(byTrackID: CMPersistentTrackID) -> AVTimedMetadataGroup?

Returns a source timed metadata group for the track that contains the specified identifier.

### Finishing the Request

func finish(withComposedVideoFrame: CVPixelBuffer)

Finishes the request to compose the frame.

func finish(with: any Error)

Finishes the request with an error.

func finishCancelledRequest()

Cancels the request to compose a video frame.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Rendering the Composition

func startRequest(AVAsynchronousVideoCompositionRequest)

Directs a custom video compositor object to create a new pixel buffer composed asynchronously from a collection of sources.

**Required**

func cancelAllPendingVideoCompositionRequests()

Directs a custom video compositor object to cancel or finish all pending video composition requests.

