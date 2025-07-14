

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  sourceSampleBuffer(byTrackID:) 

Instance Method

# sourceSampleBuffer(byTrackID:)

Returns a source sample buffer for the track that contains the specified identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func sourceSampleBuffer(byTrackID trackID: CMPersistentTrackID) -> CMSampleBuffer?
```

## Parameters 

`trackID`  

The identifier of the track that contains the source sample data.

## Return Value

A sample buffer, or `nil` if not found.

## See Also

### Accessing Source Data

var sourceTrackIDs: [NSNumber]

The identifiers of tracks that contain source video.

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of tracks that contain source sample data.

func sourceFrame(byTrackID: CMPersistentTrackID) -> CVPixelBuffer?

Returns a source pixel buffer for the track that contains the specified identifier.

func sourceTimedMetadata(byTrackID: CMPersistentTrackID) -> AVTimedMetadataGroup?

Returns a source timed metadata group for the track that contains the specified identifier.

