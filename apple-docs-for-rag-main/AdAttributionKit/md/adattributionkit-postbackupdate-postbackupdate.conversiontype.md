

- AdAttributionKit
- PostbackUpdate
-  PostbackUpdate.ConversionType 

Enumeration

# PostbackUpdate.ConversionType

Values that describe the types of conversions.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
enum ConversionType
```

## Topics

### Enumeration Cases

case install

The value that represents the installation of an app after an ad interaction.

case reengagement

The value that represents someone reengaging with an app they’ve previously installed.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

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
- Sendable

