

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.Chirality 

Enumeration

# AnchoringComponent.Target.Chirality

Defines the chirality of tracked hands to look for.

Mac Catalyst 14.0+visionOS 1.0+

``` source
enum Chirality
```

## Topics

### Operators

static func == (AnchoringComponent.Target.Chirality, AnchoringComponent.Target.Chirality) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case either

case left

case right

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

## See Also

### Hand tracking

Happy Beam

Leverage a Full Space to create a fun game using ARKit.

struct HandLocation

Defines the locations of tracked hands to look for.

