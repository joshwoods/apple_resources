

- PHASE
-  PHASEAsset 

Class

# PHASEAsset

A base class that adds a name to framework assets.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEAsset
```

## Overview

Through inheritance, this class adds a string identifier to subclasses, for example, PHASESoundAsset and PHASESoundEventNodeAsset.

PHASE generates objects of this type based on template PHASEDefinition subclasses. For example, PHASE gives you a PHASESoundEventNodeAsset when you register a PHASESoundEventNodeDefinition with the asset registry via registerSoundEventAsset(rootNode:identifier:).

## Topics

### Identifying an Asset

var identifier: String

A unique name for the asset.

### Classifying an Asset

enum AssetType

Options that determine how PHASE manages sound assets in memory.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASEGlobalMetaParameterAsset
- PHASESoundAsset
- PHASESoundEventNodeAsset

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Selection and Playback

class PHASESoundAsset

A sound resource stored in the asset registry.

class PHASESoundEvent

An object that determines which audio to play.

enum RenderingState

The playback status of audio.

class PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

class PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

