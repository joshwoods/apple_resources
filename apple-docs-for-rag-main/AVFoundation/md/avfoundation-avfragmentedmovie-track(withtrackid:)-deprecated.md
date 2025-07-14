

- AVFoundation
- AVFragmentedMovie
-  track(withTrackID:) Deprecated

Instance Method

# track(withTrackID:)

Retrieves a track in the movie that contains the specified identifier.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVFragmentedMovieTrack?
```

Deprecated

Use loadTrack(withTrackID:) instead

## Parameters 

`trackID`  

The persistent track identifier.

## Return Value

A movie track, or `nil` if there is no track with the identifier.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load a track asynchronously using loadTrack(withTrackID:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVFragmentedMovieTrack]

The tracks that a movie contains.

func tracks(withMediaType: AVMediaType) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

