

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  sourceSampleDataTrackIDs 

Instance Property

# sourceSampleDataTrackIDs

The identifiers of tracks that contain source sample data.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@nonobjc
var sourceSampleDataTrackIDs: [CMPersistentTrackID] { get }
```

## Discussion

Sample data tracks have a media type of kCMMediaType_Metadata.

## See Also

### Accessing Source Data

var sourceTrackIDs: [NSNumber]

The identifiers of tracks that contain source video.

func sourceFrame(byTrackID: CMPersistentTrackID) -> CVPixelBuffer?

Returns a source pixel buffer for the track that contains the specified identifier.

func sourceSampleBuffer(byTrackID: CMPersistentTrackID) -> CMSampleBuffer?

Returns a source sample buffer for the track that contains the specified identifier.

func sourceTimedMetadata(byTrackID: CMPersistentTrackID) -> AVTimedMetadataGroup?

Returns a source timed metadata group for the track that contains the specified identifier.

