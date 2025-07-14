

- GameplayKit
-  GKComponent 

Class

# GKComponent

The abstract superclass for creating objects that add specific gameplay functionality to an entity.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKComponent
```

## Overview

GKComponent is the abstract superclass for custom component classes you create when building a game with Entity-Component architecture. In this architecture, an *entity* is an object relevant to the game, and a *component* is an object that handles specific aspects of an entity’s behavior in a general way. Because a component’s scope of functionality is limited, you can reuse the same component class for many different kinds of entities.

You create components by subclassing GKComponent to implement reusable behavior. Then, you build game entities by creating GKEntity objects and using the addComponent(_:) method to attach instances of your custom component classes.

At runtime, a component-based game needs to dispatch periodic logic—from an update/render loop method such as update(_:) (SpriteKit) or renderer(_:updateAtTime:) (SceneKit), or a CADisplayLink (iOS) or CVDisplayLink (macOS) timer in a custom rendering engine—to each of its components. GameplayKit provides two mechanisms for dispatching updates:

- Per-entity. Call each entity’s update(deltaTime:) method, which will then forward to the update(deltaTime:) method of each component. This option can be quickly implemented in games with a small number of entities and components.

- Per-component. Use a GKComponentSystem object to handle all instances of a specific component class. When you call a component system’s update(deltaTime:) method, it forwards to the update(deltaTime:) method of all the component objects it manages. Because a component system needs no knowledge of your game’s entity/component hierarchy, this option works well for games with complex object graphs.

For more information on Entity-Component architecture, read Entities and Components in GameplayKit Programming Guide.

## Topics

### Performing Periodic Updates

func update(deltaTime: TimeInterval)

Performs any custom periodic actions defined by the component subclass.

### Working with Entities

var entity: GKEntity?

The entity that owns this component.

func didAddToEntity()

Notifies the component that it has been assigned to an entity.

func willRemoveFromEntity()

Notifies the component that it has been removed from an entity.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKAgent
- GKSCNNodeComponent
- GKSKNodeComponent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Entities and Components

class GKEntity

An object relevant to gameplay, with functionality entirely provided by a collection of component objects.

class GKComponentSystem

Manages periodic update messages for all component objects of a specified class.

