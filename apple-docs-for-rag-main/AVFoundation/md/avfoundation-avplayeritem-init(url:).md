

- AVFoundation
- AVPlayerItem
-  init(url:) 

Initializer

# init(url:)

Creates a player item with a specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
convenience init(url URL: URL)
```

## Parameters 

`URL`  

A URL identifying the media resource to be played.

## Return Value

A new player item, prepared to use `URL`.

## Discussion

This method immediately returns the item, but with the status AVPlayerItem.Status.unknown.

Associating the player item with an AVPlayer immediately begins enqueuing its media and preparing it for playback. If the URL contains valid data that can be used by the player item, its status later changes to AVPlayerItem.Status.readyToPlay. If the URL contains no valid data or otherwise can’t be used by the player item, its status later changes to AVPlayerItem.Status.failed. You can determine the nature of the failure by querying the player item’s error property.

## See Also

### Creating a Player Item

convenience init(asset: AVAsset)

Creates a player item for a specified asset.

convenience init(asset: any AVAsset &amp; Sendable)

convenience init(asset: AVAsset, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

Creates a player item for the asset, and automatically loads values for the specified properties.

convenience init(asset: any AVAsset &amp; Sendable, automaticallyLoadedAssetKeys: [AVPartialAsyncProperty&lt;AVAsset>])

init(asset: AVAsset, automaticallyLoadedAssetKeys: [String]?)

Creates a player item with the specified asset and the asset keys to automatically load.

