

- AVFoundation
- AVPlayerItem
-  automaticallyLoadedAssetKeys 

Instance Property

# automaticallyLoadedAssetKeys

The array of asset keys to be automatically loaded before the player item is ready to play.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var automaticallyLoadedAssetKeys: [String] { get }
```

## Discussion

The value of each key in `automaticallyLoadedAssetKeys` will automatically be loaded by the asset prior to the player item reaching a status of AVPlayerItem.Status.readyToPlay. When this status is reached, the asset’s statusOfValue(forKey:error:) method returns AVKeyValueStatus.loaded for the status of all keys in the array. If loading of any of the asset’s key values fails, the player item’s status will change to AVPlayerItem.Status.failed.

## See Also

### Accessing Initialization Parameters

var asset: AVAsset

The asset provided during initialization.

