

- RealityKit
-  PhysicsBodyParameterTypes 

Structure

# PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsBodyParameterTypes
```

## Topics

### Initializers

init(rawValue: UInt32)

### Instance Properties

let rawValue: UInt32

The backing storage for force effect inputs.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let angularVelocity: PhysicsBodyParameterTypes

The angular velocity of each rigid body.

static let distance: PhysicsBodyParameterTypes

The distance of each rigid body from the effect origin.

static let inertiaTensor: PhysicsBodyParameterTypes

The inertia tensor of each rigid body.

static let mass: PhysicsBodyParameterTypes

The mass of each rigid body,

static let orientation: PhysicsBodyParameterTypes

The orientation of each rigid body relative to the effect orientation.

static let position: PhysicsBodyParameterTypes

The center of mass of each rigid body relative to the effect origin.

static let velocity: PhysicsBodyParameterTypes

The linear velocity of each rigid body.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Updating effects

func update(parameters: inout ForceEffectParameters)

Defines how the custom force effect computes forces at each physics simulation step.

**Required** Default implementation provided.

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Registers the custom effect.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

struct UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

