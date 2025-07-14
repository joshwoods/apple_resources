

- GameplayKit
-  GKEntity 

Class

# GKEntity

An object relevant to gameplay, with functionality entirely provided by a collection of component objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKEntity
```

## Overview

A GKEntity object represents an entity in games with Entity-Component architecture. In this design, an *entity* is a general type for objects relevant to the game. Entities typically define no functionality of their own—instead, you define an entity’s features through composition, by adding *components* that each handle specific aspects of an entity’s behavior in a general way. Because components (GKComponent subclasses) are general and reusable, you can add many kinds of entities to a game by combining components in different ways, without needing to design new entity classes.

For more information on Entity-Component architecture, read Entities and Components in GameplayKit Programming Guide.

## Topics

### Creating an Entity

init()

Initializes a new entity object.

### Managing an Entity’s List of Components

var components: [GKComponent]

The entity’s list of components.

func addComponent(GKComponent)

Adds a component to the entity.

### Performing Periodic Updates

func update(deltaTime: TimeInterval)

Performs periodic updates for each of the entity’s components.

### Instance Methods

func component&lt;ComponentType>(ofType: ComponentType.Type) -> ComponentType?

func removeComponent&lt;ComponentType>(ofType: ComponentType.Type)

## Relationships

### Inherits From

- NSObject

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

class GKComponent

The abstract superclass for creating objects that add specific gameplay functionality to an entity.

class GKComponentSystem

Manages periodic update messages for all component objects of a specified class.

