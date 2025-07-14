

- AVFoundation
- AVComposition
-  unusedTrackID() 

Instance Method

# unusedTrackID()

Returns an identifier that no other tracks in the asset use.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func unusedTrackID() -> CMPersistentTrackID
```

## Return Value

An unused CMPersistentTrackID value.

## See Also

### Accessing Tracks

var tracks: [AVCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]

Returns tracks that contain media of a specified characteristic.

