

- AVFoundation
- AVMovie
-  tracks(withMediaCharacteristic:) Deprecated

Instance Method

# tracks(withMediaCharacteristic:)

Retrieves tracks in the movie that present media of the specified characteristic.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func tracks(withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> [AVMovieTrack]
```

Deprecated

Use loadTracks(withMediaCharacteristic:completionHandler:) instead.

## Parameters 

`mediaCharacteristic`  

The media characteristic of the tracks to return.

## Return Value

An array of tracks, which is empty if there are no tracks with the media characteristic.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaCharacteristic:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

