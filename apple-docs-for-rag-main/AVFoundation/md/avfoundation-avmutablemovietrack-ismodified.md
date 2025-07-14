

- AVFoundation
- AVMutableMovieTrack
-  isModified 

Instance Property

# isModified

A Boolean value that indicates whether a track is in a modified state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var isModified: Bool { get set }
```

## Discussion

This property is `YES` when the `AVMutableMovieTrack` object has been modified since it was created, was last written, or had its modified state cleared.

## See Also

### Configuring Track Information

var alternateGroupID: Int

A number that identifies the track as a member of a particular alternate group.

var mediaDataStorage: AVMediaDataStorage?

A storage container for the media data to be added to a track.

var sampleReferenceBaseURL: URL?

The base URL for sample references.

