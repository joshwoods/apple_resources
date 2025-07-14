

- RealityKit
-  PhysicsMassProperties 

Structure

# PhysicsMassProperties

Mass properties of a physics body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct PhysicsMassProperties
```

## Topics

### Using default mass properties

static let `default`: PhysicsMassProperties

The default mass properties, equivalent to a unit sphere with a mass of 1 kilogram.

### Creating custom mass properties

init()

Creates a mass properties instance with default settings.

init(mass: Float, inertia: SIMD3&lt;Float>, centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf))

Creates a mass properties instance with the given settings.

init(shape: ShapeResource, density: Float)

Creates the mass properties for a solid shape with the specified density.

init(shape: ShapeResource, mass: Float)

Creates the mass properties for a solid shape with the specified mass.

### Getting mass properties

var mass: Float

The mass in kilograms.

var inertia: SIMD3&lt;Float>

The inertia in kilograms per square meter.

var centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf)

The position of the center of mass and the orientation of the principal axes.

### Comparing mass properties

static func == (PhysicsMassProperties, PhysicsMassProperties) -> Bool

Indicates whether two physics mass properties are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Physical properties

struct PhysicsBodyComponent

A component that defines an entity’s behavior in physics body simulations.

class PhysicsMaterialResource

Material properties, like friction, of a physically simulated object.

enum PhysicsBodyMode

The ways that a physics body can move in response to physical forces.

