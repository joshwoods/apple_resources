

- PHASE
- PHASEAssetRegistry
-  asset(forIdentifier:) 

Instance Method

# asset(forIdentifier:)

Provides the asset named with the designated identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func asset(forIdentifier identifier: String) -> PHASEAsset?
```

## Parameters 

`identifier`  

The unique name of the asset.

## Return Value

A framework asset by the destignated name, if the app registers the asset prior. Otherwise, returns `nil`.

## See Also

### Registering Sound Event Assets

func registerSoundEventAsset(rootNode: PHASESoundEventNodeDefinition, identifier: String?) throws -> PHASESoundEventNodeAsset

Registers the root node of the sound event asset.

