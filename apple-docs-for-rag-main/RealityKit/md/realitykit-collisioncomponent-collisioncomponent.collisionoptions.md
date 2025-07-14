

- RealityKit
- CollisionComponent
-  CollisionComponent.CollisionOptions 

Structure

# CollisionComponent.CollisionOptions

The options set that defines how a collision object reports collisions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct CollisionOptions
```

## Topics

### Initializers

init(rawValue: UInt)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let fullContactInformation: CollisionComponent.CollisionOptions

Reports full contact information for collision events.

static let none: CollisionComponent.CollisionOptions

An option that reports the default collision information with dynamic collision objects.

static let `static`: CollisionComponent.CollisionOptions

Omits reporting collisions with static collision objects.

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

