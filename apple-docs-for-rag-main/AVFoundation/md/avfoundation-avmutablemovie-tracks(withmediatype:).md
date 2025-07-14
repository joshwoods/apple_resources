

- AVFoundation
- AVMutableMovie
-  tracks(withMediaType:) 

Instance Method

# tracks(withMediaType:)

Retrieves tracks in the movie that present media of the specified type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVMutableMovieTrack]
```

## Parameters 

`mediaType`  

The media type of the tracks to return.

## Return Value

An array of tracks, which is empty if there are no tracks with the media type.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaType:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMutableMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableMovieTrack]

Retrieve tracks in the movie that present media of the specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

