

- AVFoundation
- AVPartialAsyncProperty
-  tracks 

Type Property

# tracks

The tracks of media that an asset contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var tracks: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Tracks

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVAssetTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

func findUnusedTrackID(completionHandler: (CMPersistentTrackID, (any Error)?) -> Void)

Loads an identifier that no other track in the asset uses.

