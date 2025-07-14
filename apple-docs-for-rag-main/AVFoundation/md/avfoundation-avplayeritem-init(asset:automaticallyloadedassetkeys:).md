

- AVFoundation
- AVPlayerItem
-  init(asset:automaticallyLoadedAssetKeys:) 

Initializer

# init(asset:automaticallyLoadedAssetKeys:)

Creates a player item with the specified asset and the asset keys to automatically load.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
init(
    asset: AVAsset,
    automaticallyLoadedAssetKeys: [String]?
)
```

## Parameters 

`asset`  

An instance of AVAsset.

`automaticallyLoadedAssetKeys`  

An array of strings, each representing a property defined by AVAsset.

## Return Value

An initialized instance of `AVPlayerItem`.

## Discussion

The value of each key in `automaticallyLoadedAssetKeys` will automatically be loaded by the underlying AVAsset before the player item achieves the status AVPlayerItem.Status.readyToPlay; i.e. when the item is ready to play, the value returned by invoking the asset property’s statusOfValue(forKey:error:) method will be one of the terminal status values, either AVKeyValueStatus.loaded, AVKeyValueStatus.failed, or AVKeyValueStatus.cancelled.

## See Also

### Creating a Player Item

convenience init(url: URL)

Creates a player item with a specified URL.

convenience init(asset: AVAsset)

Creates a player item for a specified asset.

convenience init(asset: any AVAsset &amp; Sendable)

convenience init(asset: AVAsset, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

Creates a player item for the asset, and automatically loads values for the specified properties.

convenience init(asset: any AVAsset &amp; Sendable, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

