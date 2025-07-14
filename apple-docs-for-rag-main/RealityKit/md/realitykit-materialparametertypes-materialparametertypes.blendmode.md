

- RealityKit
- MaterialParameterTypes
-  MaterialParameterTypes.BlendMode 

Enumeration

# MaterialParameterTypes.BlendMode

Modes that describe how materials should be blended with content behind them.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum BlendMode
```

## Topics

### Operators

static func == (MaterialParameterTypes.BlendMode, MaterialParameterTypes.BlendMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case add

Blend by adding the material’s color to the background color, ignoring alpha.

case alpha

Blend by multiplying the material’s color value by its alpha value

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

