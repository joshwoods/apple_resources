

- PHASE
-  PHASEContainerNodeDefinition 

Class

# PHASEContainerNodeDefinition

A node that plays all its children at the same time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEContainerNodeDefinition
```

## Overview

This node adds structure to the sound event tree while performing no conditional logic or audio playback of its own. By passing invocation to all its children at once, this class invokes the child nodes’ actions simultaneously.

## Topics

### Creating a Node

init()

Creates a container node.

init(identifier: String)

Creates a container node with the given name.

class func new() -> Self

Creates a container node.

### Adding Descendent Nodes

func addSubtree(PHASESoundEventNodeDefinition)

Adds a sound event node as a child.

## Relationships

### Inherits From

- PHASESoundEventNodeDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Control Nodes

class PHASESwitchNodeDefinition

A node that passes invocation to only one of its child nodes.

class PHASERandomNodeDefinition

A sound event node that invokes one of its child nodes at random.

class PHASEBlendNodeDefinition

A node that smoothly fades between the audio of its child nodes.

