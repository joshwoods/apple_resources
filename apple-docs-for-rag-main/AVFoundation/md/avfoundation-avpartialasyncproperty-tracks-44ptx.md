

- AVFoundation
- AVPartialAsyncProperty
-  tracks 

Type Property

# tracks

The tracks an asset contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var tracks: AVAsyncProperty { get }
```

Available when `Root` inherits `AVURLAsset`.

## Mentioned in 

Loading media data asynchronously

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Tracks

func findCompatibleTrack(for: AVCompositionTrack, completionHandler: (AVAssetTrack?, (any Error)?) -> Void)

Loads an asset track from which you can insert any time range into the composition track.

