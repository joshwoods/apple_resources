

- RealityKit
- CharacterControllerComponent
-  CharacterControllerComponent.CollisionFlags 

Structure

# CharacterControllerComponent.CollisionFlags

An option set that specifies which parts of the character capsule have collided with other objects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct CollisionFlags
```

## Topics

### Initializers

init(rawValue: UInt8)

Initializes collisions flags from a raw value.

### Instance Properties

let rawValue: UInt8

The bitmask representation of the option set.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let bottom: CharacterControllerComponent.CollisionFlags

The bottom of capsule was hit when moving in the down direction.

static let none: CharacterControllerComponent.CollisionFlags

No collision.

static let side: CharacterControllerComponent.CollisionFlags

The side of capsule was hit when moving in the direction tangent to the up vector.

static let top: CharacterControllerComponent.CollisionFlags

The top of capsule was hit when moving in the up direction.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Character control

struct CharacterControllerComponent

A component that manages character movement.

struct Collision

A container that holds collision state for the character controller.

struct CharacterControllerStateComponent

A component that represents the state of a character controller.

