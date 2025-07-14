

- RealityKit
- SceneUnderstandingComponent
-  SceneUnderstandingComponent.EntityType 

Enumeration

# SceneUnderstandingComponent.EntityType

Types of real-world objects that a scene-understanding component models.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum EntityType
```

## Topics

### Choosing the entity type

case face

An entity that models a face that the framework detects in the physical environment.

case meshChunk

An entity that models the physical shape of the environment within a given cubic region.

### Comparing entity types

static func == (SceneUnderstandingComponent.EntityType, SceneUnderstandingComponent.EntityType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Managing the component

var entityType: SceneUnderstandingComponent.EntityType?

The type of real-world objects that the component models.

static func registerComponent()

Registers a new component type.

