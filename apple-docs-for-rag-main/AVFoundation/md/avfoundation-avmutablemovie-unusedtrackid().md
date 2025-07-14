

- AVFoundation
- AVMutableMovie
-  unusedTrackID() 

Instance Method

# unusedTrackID()

Returns an identifier that no other tracks in the asset use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func unusedTrackID() -> CMPersistentTrackID
```

## Return Value

An unused CMPersistentTrackID value.

## See Also

### Accessing Tracks

var tracks: [AVMutableMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVMutableMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableMovieTrack]

Retrieve tracks in the movie that present media of the specified characteristic.

