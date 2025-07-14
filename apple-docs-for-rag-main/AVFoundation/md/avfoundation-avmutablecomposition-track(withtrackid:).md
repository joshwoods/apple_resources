

- AVFoundation
- AVMutableComposition
-  track(withTrackID:) 

Instance Method

# track(withTrackID:)

Returns a track that contains the specified identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVMutableCompositionTrack?
```

## Parameters 

`trackID`  

The persistent track identifier.

## Return Value

A composition track or `nil` if no track is available.

## Discussion

Apple discourages using this method. Load a track asynchronously using loadTrack(withTrackID:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMutableCompositionTrack]

The tracks that a composition contains.

func tracks(withMediaType: AVMediaType) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified characteristic.

