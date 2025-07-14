

- PHASE
-  PHASESoundEventNodeAsset 

Class

# PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESoundEventNodeAsset
```

## Overview

This object refers by name to a collection of sound event nodes that connect to form a tree, or hierarchy. To retrieve an instance of this class, add a sound-event node definition to the asset registry using registerSoundEventAsset(rootNode:identifier:). Choose the `rootNode` argument from the subclasses in Sound Event Nodes based on the playback features your app requires.

To play a single audio asset, register a `rootNode` with only one audio-providing node. Alternatively, to create a sound event that can change its audio based on your app’s current state, register a `rootNode` that contains children. By adding multiple nodes that play varying audio as children to a control node, PHASE plays the right audio for the moment based on control logic that you define.

To create a playable sound event from this class, pass identifier to the `assetIdentifier` parameter of the sound event intializer, init(engine:assetIdentifier:). Then, invoke the sound event by calling start(completion:).

As an opaque derived object, this class adds no properties to its base class.

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

class PHASESoundAsset

A sound resource stored in the asset registry.

class PHASESoundEvent

An object that determines which audio to play.

enum RenderingState

The playback status of audio.

class PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

class PHASEAsset

A base class that adds a name to framework assets.

Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

