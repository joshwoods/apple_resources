

- AVFoundation
- AVPlayerItem
-  init(asset:automaticallyLoadedAssetKeys:) 

Initializer

# init(asset:automaticallyLoadedAssetKeys:)

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
convenience init(
    asset: any AVAsset & Sendable,
    automaticallyLoadedAssetKeys: [AVPartialAsyncProperty]
)
```

## See Also

### Creating a Player Item

convenience init(url: URL)

Creates a player item with a specified URL.

convenience init(asset: AVAsset)

Creates a player item for a specified asset.

convenience init(asset: any AVAsset &amp; Sendable)

convenience init(asset: AVAsset, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

Creates a player item for the asset, and automatically loads values for the specified properties.

init(asset: AVAsset, automaticallyLoadedAssetKeys: [String]?)

Creates a player item with the specified asset and the asset keys to automatically load.

