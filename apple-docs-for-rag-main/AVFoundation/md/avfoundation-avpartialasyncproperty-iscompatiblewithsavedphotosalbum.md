

- AVFoundation
- AVPartialAsyncProperty
-  isCompatibleWithSavedPhotosAlbum 

Type Property

# isCompatibleWithSavedPhotosAlbum

A Boolean value that indicates whether you can write the asset to the Saved Photos album.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS 1.0+

``` source
static var isCompatibleWithSavedPhotosAlbum: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Suitability

static var isPlayable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether an asset contains playable content.

static var isExportable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can export an asset using an export session.

static var isReadable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

static var isComposable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can use the asset in a media composition.

static var isCompatibleWithAirPlayVideo: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

