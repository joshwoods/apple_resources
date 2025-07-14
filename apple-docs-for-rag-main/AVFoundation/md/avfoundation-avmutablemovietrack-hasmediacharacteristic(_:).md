

- AVFoundation
- AVMutableMovieTrack
-  hasMediaCharacteristic(\_:) 

Instance Method

# hasMediaCharacteristic(\_:)

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func hasMediaCharacteristic(_ mediaCharacteristic: AVMediaCharacteristic) -> Bool
```

## Parameters 

`mediaCharacteristic`  

The media characteristic of interest.

## Return Value

true if the track references media with the specified characteristic; otherwise, false.

## See Also

### Accessing Track Information

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

var isDecodable: Bool

A Boolean value that indicates whether the track is decodable in the current environment.

var isEnabled: Bool

A Boolean value that indicates whether the track’s container enables it.

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

var hasProtectedContent: Bool

A Boolean value that indicates whether a track contains protected content.

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

