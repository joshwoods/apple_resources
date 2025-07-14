

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  sourceTrackIDs 

Instance Property

# sourceTrackIDs

The identifiers of tracks that contain source video.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var sourceTrackIDs: [NSNumber] { get }
```

## See Also

### Accessing Source Data

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of tracks that contain source sample data.

func sourceFrame(byTrackID: CMPersistentTrackID) -> CVPixelBuffer?

Returns a source pixel buffer for the track that contains the specified identifier.

func sourceSampleBuffer(byTrackID: CMPersistentTrackID) -> CMSampleBuffer?

Returns a source sample buffer for the track that contains the specified identifier.

func sourceTimedMetadata(byTrackID: CMPersistentTrackID) -> AVTimedMetadataGroup?

Returns a source timed metadata group for the track that contains the specified identifier.

