

- PHASE
- PHASEAssetRegistry
-  registerSoundEventAsset(rootNode:identifier:) 

Instance Method

# registerSoundEventAsset(rootNode:identifier:)

Registers the root node of the sound event asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func registerSoundEventAsset(
    rootNode: PHASESoundEventNodeDefinition,
    identifier: String?
) throws -> PHASESoundEventNodeAsset
```

## Parameters 

`rootNode`  

The root node of the sound event asset to register.

`identifier`  

The identifier to assign to this parameter. Assigning `nil` generates an automatic identifier.

## Return Value

A sound event node asset.

## See Also

### Registering Sound Event Assets

func asset(forIdentifier: String) -> PHASEAsset?

Provides the asset named with the designated identifier.

