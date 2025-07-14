

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Program
-  PhysicallyBasedMaterial.Program.Descriptor 

Structure

# PhysicallyBasedMaterial.Program.Descriptor

Specifies all parameters necessary to initialize `PhysicallyBasedMaterial` programs

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Descriptor
```

## Topics

### Operators

static func == (PhysicallyBasedMaterial.Program.Descriptor, PhysicallyBasedMaterial.Program.Descriptor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

### Instance Properties

var blendMode: MaterialParameterTypes.BlendMode?

Describes how materials using the created `PhysicallyBasedMaterial.Program` will be blended with content behind them.

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

