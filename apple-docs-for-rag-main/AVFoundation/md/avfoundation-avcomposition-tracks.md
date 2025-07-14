

- AVFoundation
- AVComposition
-  tracks 

Instance Property

# tracks

The tracks that a composition contains.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var tracks: [AVCompositionTrack] { get }
```

## See Also

### Accessing Tracks

func track(withTrackID: CMPersistentTrackID) -> AVCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]

Returns tracks that contain media of a specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

