

- RealityKit
-  RadialForceEffect 

Structure

# RadialForceEffect

A force effect that pulls objects toward its center with a spring-like (distance dependent) force.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct RadialForceEffect
```

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(strength: Double, restDistance: Double)

Creates a radial force effect.

### Instance Properties

var forceMode: ForceMode

The type of force this effect applies.

var parameterTypes: PhysicsBodyParameterTypes

The input rigid body parameters.

let restDistance: Float

A distance at which the rigid bodies receive zero radial force.

let strength: Float

The magnitude of the force.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func update(parameters: inout ForceEffectParameters)

Calculates the radial forces for rigid bodies from the force effect.

### Default Implementations

ForceEffectProtocol Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- ForceEffectProtocol

## See Also

### Built-in force effect types

struct ConstantForceEffect

A force effect that exerts a constant force in a direction relative to the effect’s transform.

struct ConstantRadialForceEffect

A force effect that pulls objects toward its center with a constant strength.

struct DragForceEffect

A force effect that slows bodies within its area of effect with a force proportional to the body’s velocity.

struct TurbulenceForceEffect

A force effect that applies random forces with magnitudes proportional to each body’s velocity.

struct VortexForceEffect

A force effect whose forces circulate around an axis centered at the origin of the effect.

