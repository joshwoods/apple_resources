

- RealityKit
-  PhysicsBodyMode 

Enumeration

# PhysicsBodyMode

The ways that a physics body can move in response to physical forces.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum PhysicsBodyMode
```

## Topics

### Setting the physics body mode

case `static`

The body never moves.

case kinematic

The user controls body movement.

case dynamic

Forces and collisions control body movement.

### Comparing modes

static func == (PhysicsBodyMode, PhysicsBodyMode) -> Bool

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

### Physical properties

struct PhysicsBodyComponent

A component that defines an entity’s behavior in physics body simulations.

class PhysicsMaterialResource

Material properties, like friction, of a physically simulated object.

struct PhysicsMassProperties

Mass properties of a physics body.

