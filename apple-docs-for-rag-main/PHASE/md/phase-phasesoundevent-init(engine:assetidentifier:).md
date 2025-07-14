

- PHASE
- PHASESoundEvent
-  init(engine:assetIdentifier:) 

Initializer

# init(engine:assetIdentifier:)

Creates a sound event node with the given asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    engine: PHASEEngine,
    assetIdentifier: String
) throws
```

## Parameters 

`engine`  

The object that controls this class’s associated audio output.

`assetIdentifier`  

The identifier for the sound event asset from which to create the node.

## See Also

### Creating a Sound Event

init(engine: PHASEEngine, assetIdentifier: String, mixerParameters: PHASEMixerParameters) throws

Creates a sound event node with the given asset and mixer parameters.

