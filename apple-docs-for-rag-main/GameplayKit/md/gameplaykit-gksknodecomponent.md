

- GameplayKit
-  GKSKNodeComponent 

Class

# GKSKNodeComponent

A component that manages a SpriteKit node.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKSKNodeComponent
```

## Overview

Adding a GKSKNodeComponent object to an entity automatically updates the entity property of the component’s SpriteKit node (an SKNode object) to point to that entity.

When you add entities and components to a node in the Xcode SpriteKit scene editor, Xcode automatically creates a GKSKNodeComponent object to manage the relationship between that SpriteKit node and the GKEntity object that node represents. Load the scene file with the GKScene class to access these entities and components.

Tip

The GKSKNodeComponent class adopts the GKAgentDelegate protocol. If you use the GKAgent2D class to drive the movement of game entities, set your GKSKNodeComponent instance as the delegate for the entity’s agent, and GameplayKit will automatically synchronize the agent and its SpriteKit representation.

For more information on Entity-Component architecture, read Entities and Components in GameplayKit Programming Guide.

## Topics

### Creating a SpriteKit Component

init(node: SKNode)

Initializes a component to manage the specified SpriteKit node.

### Accessing the Component’s SpriteKit Node

var node: SKNode

The SpriteKit node managed by the component.

## Relationships

### Inherits From

- GKComponent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKAgentDelegate
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Xcode and SpriteKit Integration

class GKScene

A container for associating GameplayKit objects with a SpriteKit scene.

protocol GKSceneRootNodeType

Identifies scene classes from other frameworks that support embedded GameplayKit information.

