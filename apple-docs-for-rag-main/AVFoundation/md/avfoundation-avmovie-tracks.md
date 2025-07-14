

- AVFoundation
- AVMovie
-  tracks 

Instance Property

# tracks

The tracks that a movie contains.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var tracks: [AVMovieTrack] { get }
```

## See Also

### Accessing Tracks

func track(withTrackID: CMPersistentTrackID) -> AVMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

