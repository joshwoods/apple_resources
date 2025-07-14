

- PHASE
-  PHASESoundEventNodeDefinition 

Class

# PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESoundEventNodeDefinition
```

## Overview

This class defines the base functionality for an object that, depending on the derived class’s type, either plays audio or hands off the invocation to one or more other nodes.

### Configure a Sound Event Node to Play Audio

To play audio with this class, retrieve a sound-event node asset (PHASESoundEventNodeAsset) that generates sound events by creating and registering one of the audio-providing node definitions in Sound Event Nodes. Call registerSoundEventAsset(rootNode:identifier:) and pass the node definition in the `rootNode` argument. Provide an `identifier` argument with a unique name that your app refers to later when generating a playable PHASESoundEvent.

### Configure a Node Hiearchy that Reacts to Your App’s State

You can create a hierarchy of nodes that blends audio based on your app’s parameters, or plays the right audio based on your app’s state. To create the hierarchy, register one of the control nodes in Sound Event Nodes by calling registerSoundEventAsset(rootNode:identifier:), passing in a unique identifier you define for the subclass.

The particular configuration you choose for a node hierarchy instructs PHASE on which audio to play, when to play it, or whether to hand off an invocation to one or more child nodes (children).

For example, if you register and invoke a PHASESwitchNodeDefinition that contains two child PHASESamplerNodeDefinition objects, PHASE plays the audio of one of the child sampler nodes based on the current value of the switch node’s metaparameter. For more information, see metaParameters.

## Topics

### Accessing Child Nodes

var children: [PHASESoundEventNodeDefinition]

An array of child sound event nodes.

### Identifying a Definition

class PHASEDefinition

A base class that adds a name to framework definitions.

## Relationships

### Inherits From

- PHASEDefinition

### Inherited By

- PHASEBlendNodeDefinition
- PHASEContainerNodeDefinition
- PHASEGeneratorNodeDefinition
- PHASERandomNodeDefinition
- PHASESwitchNodeDefinition

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

class PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

class PHASEAsset

A base class that adds a name to framework assets.

Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

