

- RoomPlan
- RoomBuilder
-  RoomBuilder.ConfigurationOptions 

Structure

# RoomBuilder.ConfigurationOptions

The configuration options for the RoomBuilder

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
struct ConfigurationOptions
```

## Topics

### Creating a configuration option

init(rawValue: Int)

Creates a configuration option with the specified raw value.

let rawValue: Int

A raw value for a configuration option.

### Choosing a configuration option

static let beautifyObjects: RoomBuilder.ConfigurationOptions

An option that instructs the captured room to enhance its look.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a room builder

init(options: RoomBuilder.ConfigurationOptions)

Creates a session with assets from RSCaptureSession

