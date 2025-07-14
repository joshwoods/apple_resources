

- AVFoundation
- AVPartialAsyncProperty
-  isComposable 

Type Property

# isComposable

A Boolean value that indicates whether you can use the asset in a media composition.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var isComposable: AVAsyncProperty { get }
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

static var isCompatibleWithAirPlayVideo: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

static var isCompatibleWithSavedPhotosAlbum: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can write the asset to the Saved Photos album.

