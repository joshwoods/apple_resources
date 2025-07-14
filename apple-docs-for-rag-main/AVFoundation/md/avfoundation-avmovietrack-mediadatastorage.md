

- AVFoundation
- AVMovieTrack
-  mediaDataStorage 

Instance Property

# mediaDataStorage

The storage container for media data added to a track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var mediaDataStorage: AVMediaDataStorage? { get }
```

## Discussion

The value of this property is an AVMediaDataStorage object that indicates the location to which the system writes media data when it’s inserted or appended.

## See Also

### Retrieving Track Information

var alternateGroupID: Int

A value that identifies the track as a member of a particular alternate group.

var mediaDecodeTimeRange: CMTimeRange

A range of decode times for the track’s media.

var mediaPresentationTimeRange: CMTimeRange

A range of presentation times for the track’s media.

