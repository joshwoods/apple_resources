

- PHASE
- PHASESoundEvent
-  PHASESoundEvent.RenderingState 

Enumeration

# PHASESoundEvent.RenderingState

The playback status of audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum RenderingState
```

## Overview

This enumeration defines the possible values of:

- A sound event’s renderingState property

- The engine’s renderingState property

## Topics

### States

case paused

A state in which sound event playback pauses.

case started

A state in which sound event playback starts.

case stopped

A state in which sound event playback stops.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Audio Selection and Playback

class PHASESoundAsset

A sound resource stored in the asset registry.

class PHASESoundEvent

An object that determines which audio to play.

class PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

class PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

class PHASEAsset

A base class that adds a name to framework assets.

Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

