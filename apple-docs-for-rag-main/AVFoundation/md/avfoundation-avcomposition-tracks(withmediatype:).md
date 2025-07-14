

- AVFoundation
- AVComposition
-  tracks(withMediaType:) 

Instance Method

# tracks(withMediaType:)

Returns tracks that contain media of a specified type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVCompositionTrack]
```

## Parameters 

`mediaType`  

The media type of the tracks to return.

## Return Value

An array of tracks, which is empty if no tracks with the media type exist.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaType:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]

Returns tracks that contain media of a specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

