

- AVFoundation
- AVMutableMovieTrack
-  nominalFrameRate 

Instance Property

# nominalFrameRate

The frame rate of the track, in frames per second.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var nominalFrameRate: Float { get }
```

## Discussion

The nominal frame rate indicates the number of frames per second for tracks that contain a full frame per media sample. For field-based (interlaced) video tracks, the value of this property indicates the field rate, not the frame rate.

## See Also

### Accessing Frame-Based Characteristics

var minFrameDuration: CMTime

The minimum duration of the track’s frames.

var requiresFrameReordering: Bool

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

