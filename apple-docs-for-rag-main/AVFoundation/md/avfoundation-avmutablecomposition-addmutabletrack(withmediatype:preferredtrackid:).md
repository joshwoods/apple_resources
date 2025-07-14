

- AVFoundation
- AVMutableComposition
-  addMutableTrack(withMediaType:preferredTrackID:) 

Instance Method

# addMutableTrack(withMediaType:preferredTrackID:)

Adds an empty track to a composition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addMutableTrack(
    withMediaType mediaType: AVMediaType,
    preferredTrackID: CMPersistentTrackID
) -> AVMutableCompositionTrack?
```

## Parameters 

`mediaType`  

The media type of the new track.

`preferredTrackID`  

The preferred track ID for the new track. The system generates a unique ID if the value you specify isn’t available. If you don’t need to specify a preferred track ID, pass kCMPersistentTrackID_Invalid, and the system generates an appropriate identifier.

## Return Value

A new mutable composition track.

## See Also

### Managing Composition Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableCompositionTrack?

Returns a composition track into which you can insert any time range of the specified asset track.

func removeTrack(AVCompositionTrack)

Removes a specified track from the composition.

