

- AVFoundation
- AVComposition
-  track(withTrackID:) 

Instance Method

# track(withTrackID:)

Returns a track that contains the specified identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVCompositionTrack?
```

## Parameters 

`trackID`  

The identifier of the track to retrieve.

## Return Value

A composition track, or `nil` if no track with the identifier exists.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load a track asynchronously using loadTrack(withTrackID:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVCompositionTrack]

The tracks that a composition contains.

func tracks(withMediaType: AVMediaType) -> [AVCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]

Returns tracks that contain media of a specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

