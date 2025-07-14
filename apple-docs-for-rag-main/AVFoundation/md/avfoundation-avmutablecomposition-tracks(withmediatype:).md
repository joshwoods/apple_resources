

- AVFoundation
- AVMutableComposition
-  tracks(withMediaType:) 

Instance Method

# tracks(withMediaType:)

Returns tracks that contain media of a specified type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVMutableCompositionTrack]
```

## Parameters 

`mediaType`  

The media type of the tracks to return.

## Return Value

An array of composition tracks, which is empty if there are no matching tracks.

## Discussion

Apple discourages using this method. Load tracks asynchronously using loadTracks(withMediaType:completionHandler:) instead.

## See Also

### Accessing Tracks

var tracks: [AVMutableCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified characteristic.

