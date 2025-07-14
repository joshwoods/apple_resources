

- RealityKit
-  ForceMode 

Enumeration

# ForceMode

The options that control how physics system applies the forces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ForceMode
```

## Overview

`ForceMode` allows you to customize how the physics system applies the force-like vector quantity that you set via setForce(_:index:) and setTorque(_:index:). For example, ForceMode.force indicates the vector quantity has the unit of force, which is the most common choice. You can use ForceMode.acceleration to exert a constant acceleration on rigid bodies regardless of their mass.

## Topics

### Operators

static func == (ForceMode, ForceMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case acceleration

A direct adjustment to a body’s linear or angular acceleration, independent of its mass or inertia.

case force

A constant force or torque applied to a body, influencing motion over time.

case impulse

A direct adjustment to a body’s linear or angular momentum.

case velocity

A direct adjustment to a body’s linear or angular velocity, independent of its mass or inertia.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Custom forces

protocol ForceEffectProtocol

A protocol that defines a custom force effect.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

protocol ForceEffectBase

The base protocol for the wrapping force effect structure containing common parameters for all force-effects.

