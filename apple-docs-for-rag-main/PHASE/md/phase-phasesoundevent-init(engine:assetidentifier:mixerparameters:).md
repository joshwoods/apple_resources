

- PHASE
- PHASESoundEvent
-  init(engine:assetIdentifier:mixerParameters:) 

Initializer

# init(engine:assetIdentifier:mixerParameters:)

Creates a sound event node with the given asset and mixer parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    engine: PHASEEngine,
    assetIdentifier: String,
    mixerParameters: PHASEMixerParameters
) throws
```

## Parameters 

`engine`  

The object that controls this class’s associated audio output.

`assetIdentifier`  

The identifier for the sound event asset from which to create the node.

`mixerParameters`  

A dictionary of spatial mixer parameters to enable. The keys match available identifiers of the object’s spatial mixers.

## See Also

### Creating a Sound Event

init(engine: PHASEEngine, assetIdentifier: String) throws

Creates a sound event node with the given asset.

