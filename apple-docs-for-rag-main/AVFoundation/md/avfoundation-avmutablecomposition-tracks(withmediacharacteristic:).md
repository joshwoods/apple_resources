

- AVFoundation
- AVMutableComposition
-  tracks(withMediaCharacteristic:) 

Instance Method

# tracks(withMediaCharacteristic:)

Returns tracks that contain media of a specified characteristic.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func tracks(withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> [AVMutableCompositionTrack]
```

## Parameters 

`mediaCharacteristic`  

The media characteristic of the tracks to return.

## Return Value

An array of composition tracks, which is empty if there are no matching tracks.

## Discussion

Apple discourages using this method. Load tracks asynchronously using loadTracks(withMediaCharacteristic:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMutableCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified type.

