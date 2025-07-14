

- AVFoundation
- AVComposition
-  tracks(withMediaCharacteristic:) 

Instance Method

# tracks(withMediaCharacteristic:)

Returns tracks that contain media of a specified characteristic.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func tracks(withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]
```

## Parameters 

`mediaCharacteristic`  

The media characteristic of the tracks to return.

## Return Value

An array of tracks, which is empty if no tracks with the media characteristic exist.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaCharacteristic:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVCompositionTrack]

Returns tracks that contain media of a specified type.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

