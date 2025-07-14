

- RealityKit
- UnlitMaterial
- UnlitMaterial.Program
-  UnlitMaterial.Program.Descriptor 

Structure

# UnlitMaterial.Program.Descriptor

An object that specifies all parameters necessary to initialize `UnlitMaterial` programs

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Descriptor
```

## Topics

### Operators

static func == (UnlitMaterial.Program.Descriptor, UnlitMaterial.Program.Descriptor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

### Instance Properties

var applyPostProcessToneMap: Bool

A Boolean value that determines whether RealityKit will tonemap the output of this material.

var blendMode: MaterialParameterTypes.BlendMode?

Modes that describe how materials using the created `UnlitMaterial.Program` will be blended with content behind them.

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

