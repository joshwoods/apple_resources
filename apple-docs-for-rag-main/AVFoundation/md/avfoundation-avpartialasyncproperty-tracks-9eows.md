

- AVFoundation
- AVPartialAsyncProperty
-  tracks 

Type Property

# tracks

The tracks that a composition contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var tracks: AVAsyncProperty { get }
```

Available when `Root` inherits `AVComposition`.

## See Also

### Loading Tracks

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVCompositionTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

