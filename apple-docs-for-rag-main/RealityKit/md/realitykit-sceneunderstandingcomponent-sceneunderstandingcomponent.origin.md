

- RealityKit
- SceneUnderstandingComponent
-  SceneUnderstandingComponent.Origin 

Enumeration

# SceneUnderstandingComponent.Origin

Types of scene-understanding origins this component lives in.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Origin
```

## Topics

### Operators

static func == (SceneUnderstandingComponent.Origin, SceneUnderstandingComponent.Origin) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case system

A scene-understanding component that is owned and created by the system. Component of this origin type will model an object in real world environment.

case user

A scene-understanding component that is owned and created by the developer. Component of this origin type will model an object in virtual environment.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

