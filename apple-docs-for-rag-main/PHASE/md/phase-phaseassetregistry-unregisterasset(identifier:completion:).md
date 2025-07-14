

- PHASE
- PHASEAssetRegistry
-  unregisterAsset(identifier:completion:) 

Instance Method

# unregisterAsset(identifier:completion:)

Deallocates system memory for a given asset and removes it from the engine’s list of registered assets.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func unregisterAsset(
    identifier: String,
    completion handler: ((Bool) -> Void)? = nil
)
```

``` source
func unregisterAsset(identifier: String) async -> Bool
```

## Parameters 

`identifier`  

The unique name that the app defines for the sound asset.

`handler`  

Code that the system runs after it unregisters the asset.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func unregisterAsset(identifier: String) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Registering Sound Assets

func registerSoundAsset(url: URL, identifier: String?, assetType: PHASEAsset.AssetType, channelLayout: AVAudioChannelLayout?, normalizationMode: PHASENormalizationMode) throws -> PHASESoundAsset

Loads a sound asset from the argument URL and adds it to the engine’s list of registered assets.

func registerSoundAsset(data: Data, identifier: String?, format: AVAudioFormat, normalizationMode: PHASENormalizationMode) throws -> PHASESoundAsset

Loads a sound asset from memory and adds it to the engine’s list of registered assets.

