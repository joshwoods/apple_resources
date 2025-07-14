

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  sourceFrame(byTrackID:) 

Instance Method

# sourceFrame(byTrackID:)

Returns a source pixel buffer for the track that contains the specified identifier.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func sourceFrame(byTrackID trackID: CMPersistentTrackID) -> CVPixelBuffer?
```

## Parameters 

`trackID`  

The identifier of the track that contains the source frame.

## Return Value

A pixel buffer, or `nil` if not found.

## See Also

### Accessing Source Data

var sourceTrackIDs: [NSNumber]

The identifiers of tracks that contain source video.

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of tracks that contain source sample data.

func sourceSampleBuffer(byTrackID: CMPersistentTrackID) -> CMSampleBuffer?

Returns a source sample buffer for the track that contains the specified identifier.

func sourceTimedMetadata(byTrackID: CMPersistentTrackID) -> AVTimedMetadataGroup?

Returns a source timed metadata group for the track that contains the specified identifier.

