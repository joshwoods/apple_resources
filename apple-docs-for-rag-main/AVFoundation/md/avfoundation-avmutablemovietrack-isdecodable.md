

- AVFoundation
- AVMutableMovieTrack
-  isDecodable 

Instance Property

# isDecodable

A Boolean value that indicates whether the track is decodable in the current environment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
var isDecodable: Bool { get }
```

## Discussion

When this property is true, the system can decode the track, even if decoding may be too slow for real-time playback.

## See Also

### Accessing Track Information

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

var isEnabled: Bool

A Boolean value that indicates whether the track’s container enables it.

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

var hasProtectedContent: Bool

A Boolean value that indicates whether a track contains protected content.

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

