

- AVFoundation
- AVPartialAsyncProperty
-  segments 

Type Property

# segments

The time mappings from the track’s media samples to its timeline.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var segments: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Track Segments

func loadSegment(forTrackTime: CMTime, completionHandler: (AVAssetTrackSegment?, (any Error)?) -> Void)

Loads a segment with a target time range that contains, or is closest to, the specified track time.

func loadSamplePresentationTime(forTrackTime: CMTime, completionHandler: (CMTime, (any Error)?) -> Void)

Loads a sample presentation time that maps to the specified track time.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

