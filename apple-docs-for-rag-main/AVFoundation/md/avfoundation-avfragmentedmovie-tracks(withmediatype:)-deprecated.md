

- AVFoundation
- AVFragmentedMovie
-  tracks(withMediaType:) Deprecated

Instance Method

# tracks(withMediaType:)

Retrieves tracks in the movie that present media of the specified type.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVFragmentedMovieTrack]
```

Deprecated

Use loadTracks(withMediaType:) instead

## Parameters 

`mediaType`  

The media type of the tracks to return.

## Return Value

An array of tracks, which is empty if there are no tracks with the media type.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaType:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVFragmentedMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

