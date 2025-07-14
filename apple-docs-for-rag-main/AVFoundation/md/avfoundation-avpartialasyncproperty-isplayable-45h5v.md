

- AVFoundation
- AVPartialAsyncProperty
-  isPlayable 

Type Property

# isPlayable

A Boolean value that indicates whether an asset contains playable content.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var isPlayable: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

Note

You can attempt playback when value is false, but this may result in a substandard playback experience.

## See Also

### Loading Suitability

static var isExportable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can export an asset using an export session.

static var isReadable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

static var isComposable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can use the asset in a media composition.

static var isCompatibleWithAirPlayVideo: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

static var isCompatibleWithSavedPhotosAlbum: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can write the asset to the Saved Photos album.

