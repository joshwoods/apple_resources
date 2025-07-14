

- AVFoundation
- AVMutableMovie
-  track(withTrackID:) 

Instance Method

# track(withTrackID:)

Retrieves a track in the movie that contains the specified identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVMutableMovieTrack?
```

## Parameters 

`trackID`  

The track identifier for the requested track.

## Return Value

A movie track, or `nil` if there is no track with the identifier.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load a track asynchronously using loadTrack(withTrackID:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMutableMovieTrack]

The tracks that a movie contains.

func tracks(withMediaType: AVMediaType) -> [AVMutableMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableMovieTrack]

Retrieve tracks in the movie that present media of the specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

