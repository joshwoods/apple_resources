

- AVFoundation
- AVMutableComposition
-  tracks 

Instance Property

# tracks

The tracks that a composition contains.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var tracks: [AVMutableCompositionTrack] { get }
```

## Discussion

In a mutable composition, the tracks are instances of AVMutableCompositionTrack, whereas in AVComposition the tracks are instances of AVCompositionTrack.

## See Also

### Accessing Tracks

func track(withTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified characteristic.

