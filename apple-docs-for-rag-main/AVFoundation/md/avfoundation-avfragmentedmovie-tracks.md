

- AVFoundation
- AVFragmentedMovie
-  tracks 

Instance Property

# tracks

The tracks that a movie contains.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var tracks: [AVFragmentedMovieTrack] { get }
```

## See Also

### Accessing Tracks

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

