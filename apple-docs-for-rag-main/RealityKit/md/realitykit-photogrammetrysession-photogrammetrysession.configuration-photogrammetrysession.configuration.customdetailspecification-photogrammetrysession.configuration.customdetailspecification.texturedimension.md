

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureDimension 

Enumeration

# PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureDimension

One of the discrete texture dimensions to specify the size of the model texture maps. For example, a `.twoK` dimension means the texture map size can be up to size 2048x2048.

Mac Catalyst 17.0+macOS 14.0+

``` source
enum TextureDimension
```

## Topics

### Enumeration Cases

case eightK

case fourK

case oneK

case sixteenK

case twoK

### Initializers

init?(rawValue: UInt)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

