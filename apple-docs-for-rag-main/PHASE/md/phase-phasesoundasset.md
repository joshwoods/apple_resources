

- PHASE
-  PHASESoundAsset 

Class

# PHASESoundAsset

A sound resource stored in the asset registry.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESoundAsset
```

## Overview

This class wraps source audio data that an app intends to play. The framework requires a mixer to play a sound asset, and sound event nodes like PHASESamplerNodeDefinition combine the asset with a mixer. To provide a sound asset to a sound-event node, refer to the asset by the `identifier` you pass into the registerSoundAsset(url:identifier:assetType:channelLayout:normalizationMode:) function.

## Topics

### Accessing Sound Data

var data: Data?

A storage buffer for the sound asset.

var url: URL?

The URL of the sound asset.

### Classifying an Asset

var type: PHASEAsset.AssetType

The type of sound asset.

## Relationships

### Inherits From

- PHASEAsset

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Selection and Playback

class PHASESoundEvent

An object that determines which audio to play.

enum RenderingState

The playback status of audio.

class PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

class PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

class PHASEAsset

A base class that adds a name to framework assets.

Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

