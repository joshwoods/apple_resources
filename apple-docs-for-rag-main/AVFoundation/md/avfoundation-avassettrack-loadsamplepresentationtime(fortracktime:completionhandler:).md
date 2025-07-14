

- AVFoundation
- AVAssetTrack
-  loadSamplePresentationTime(forTrackTime:completionHandler:) 

Instance Method

# loadSamplePresentationTime(forTrackTime:completionHandler:)

Loads a sample presentation time that maps to the specified track time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadSamplePresentationTime(
    forTrackTime trackTime: CMTime,
    completionHandler: @escaping (CMTime, (any Error)?) -> Void
)
```

``` source
func loadSamplePresentationTime(forTrackTime trackTime: CMTime) async throws -> CMTime
```

## Parameters 

`trackTime`  

The track time of the presentation time to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

time  
A CMTime value, which is invalid if the track time is out of range or if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## See Also

### Loading Track Segments

static var segments: AVAsyncProperty&lt;Root, [AVAssetTrackSegment]>

The time mappings from the track’s media samples to its timeline.

func loadSegment(forTrackTime: CMTime, completionHandler: (AVAssetTrackSegment?, (any Error)?) -> Void)

Loads a segment with a target time range that contains, or is closest to, the specified track time.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

