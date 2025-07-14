

- AVFoundation
- AVMutableComposition
-  removeTrack(\_:) 

Instance Method

# removeTrack(\_:)

Removes a specified track from the composition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeTrack(_ track: AVCompositionTrack)
```

## Parameters 

`track`  

The track to remove.

## Discussion

When you remove a track, the system sets its composition value to nil.

## See Also

### Managing Composition Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableCompositionTrack?

Returns a composition track into which you can insert any time range of the specified asset track.

func addMutableTrack(withMediaType: AVMediaType, preferredTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Adds an empty track to a composition.

