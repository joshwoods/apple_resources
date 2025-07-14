

- AVFoundation
- AVPartialAsyncProperty
-  tracks 

Type Property

# tracks

The tracks that a movie contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
static var tracks: AVAsyncProperty { get }
```

Available when `Root` inherits `AVMovie`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Tracks

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVMovieTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

