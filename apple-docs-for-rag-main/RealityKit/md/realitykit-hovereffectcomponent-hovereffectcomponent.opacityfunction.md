

- RealityKit
- HoverEffectComponent
-  HoverEffectComponent.OpacityFunction 

Enumeration

# HoverEffectComponent.OpacityFunction

The blending technique options a hover effect applies to its entity’s base material.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum OpacityFunction
```

## Topics

### Operators

static func == (HoverEffectComponent.OpacityFunction, HoverEffectComponent.OpacityFunction) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case blend

Draws the hover effect with an opacity that’s equal to the product of the entity’s base material and the shader’s output.

case full

Applies an opaque hover effect and ignores the opacity of the entity’s base material.

case mask

Applies a hover effect with full opacity when the opacity of the entity’s base material is greater than five percent.

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
- Sendable

