

- AVFoundation
- AVPlayerItem
-  init(asset:) 

Initializer

# init(asset:)

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
convenience init(asset: any AVAsset & Sendable)
```

## See Also

### Creating a Player Item

convenience init(url: URL)

Creates a player item with a specified URL.

convenience init(asset: AVAsset)

Creates a player item for a specified asset.

convenience init(asset: AVAsset, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

Creates a player item for the asset, and automatically loads values for the specified properties.

convenience init(asset: any AVAsset &amp; Sendable, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

init(asset: AVAsset, automaticallyLoadedAssetKeys: [String]?)

Creates a player item with the specified asset and the asset keys to automatically load.

