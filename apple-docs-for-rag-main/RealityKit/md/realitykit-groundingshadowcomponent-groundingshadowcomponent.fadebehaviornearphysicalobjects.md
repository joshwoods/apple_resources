

- RealityKit
- GroundingShadowComponent
-  GroundingShadowComponent.FadeBehaviorNearPhysicalObjects 

Enumeration

# GroundingShadowComponent.FadeBehaviorNearPhysicalObjects

Describes the behavior of an entity’s grounding shadow when it’s near physical objects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum FadeBehaviorNearPhysicalObjects
```

## Topics

### Operators

static func == (GroundingShadowComponent.FadeBehaviorNearPhysicalObjects, GroundingShadowComponent.FadeBehaviorNearPhysicalObjects) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case constant

A grounding shadow behavior that doesn’t fade when an entity is near physical objects.

case `default`

The default grounding shadow behavior for the device’s platform.

case fade

A grounding shadow behavior that fades when an entity is near physical objects.

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

- Copyable
- Equatable
- Hashable

