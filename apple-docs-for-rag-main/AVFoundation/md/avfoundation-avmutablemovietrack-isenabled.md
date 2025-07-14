

- AVFoundation
- AVMutableMovieTrack
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the track’s container enables it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

For file-based media, you can change its isEnabled presentation state using AVPlayerItemTrack.

## See Also

### Accessing Track Information

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

var isDecodable: Bool

A Boolean value that indicates whether the track is decodable in the current environment.

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

var hasProtectedContent: Bool

A Boolean value that indicates whether a track contains protected content.

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

