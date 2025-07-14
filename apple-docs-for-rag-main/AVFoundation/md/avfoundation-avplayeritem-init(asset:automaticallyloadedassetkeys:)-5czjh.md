

- AVFoundation
- AVPlayerItem
-  init(asset:automaticallyLoadedAssetKeys:) 

Initializer

# init(asset:automaticallyLoadedAssetKeys:)

Creates a player item for the asset, and automatically loads values for the specified properties.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
convenience init(
    asset: AVAsset,
    automaticallyLoadedAssetKeys: [AVPartialAsyncProperty] = []
)
```

## Parameters 

`asset`  

The asset to play.

`automaticallyLoadedAssetKeys`  

An array of property identifiers for which the system automatically loads a value.

## Discussion

The system automatically loads values for the specified property identifiers before the player item reaches an AVPlayerItem.Status.readyToPlay state. In this state, calling status(of:) on a specified property identifier returns a value of AVAsyncProperty.Status.loaded(_:) or AVAsyncProperty.Status.failed(_:).

## See Also

### Creating a Player Item

convenience init(url: URL)

Creates a player item with a specified URL.

convenience init(asset: AVAsset)

Creates a player item for a specified asset.

convenience init(asset: any AVAsset &amp; Sendable)

convenience init(asset: any AVAsset &amp; Sendable, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

init(asset: AVAsset, automaticallyLoadedAssetKeys: [String]?)

Creates a player item with the specified asset and the asset keys to automatically load.

