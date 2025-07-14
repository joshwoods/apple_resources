

- AVFoundation
- AVAssetTrack
-  loadSegment(forTrackTime:completionHandler:) 

Instance Method

# loadSegment(forTrackTime:completionHandler:)

Loads a segment with a target time range that contains, or is closest to, the specified track time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadSegment(
    forTrackTime trackTime: CMTime,
    completionHandler: @escaping (AVAssetTrackSegment?, (any Error)?) -> Void
)
```

``` source
func loadSegment(forTrackTime trackTime: CMTime) async throws -> AVAssetTrackSegment?
```

## Parameters 

`trackTime`  

The track time of the segment to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

segment  
The loaded track segment, or `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## Discussion

If the specified track time doesn’t map to a sample presentation time, the system returns the segment with the closest matching time.

## See Also

### Loading Track Segments

static var segments: AVAsyncProperty&lt;Root, [AVAssetTrackSegment]>

The time mappings from the track’s media samples to its timeline.

func loadSamplePresentationTime(forTrackTime: CMTime, completionHandler: (CMTime, (any Error)?) -> Void)

Loads a sample presentation time that maps to the specified track time.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

