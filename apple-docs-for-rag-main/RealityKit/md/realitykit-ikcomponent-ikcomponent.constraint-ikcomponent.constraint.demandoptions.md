

- RealityKit
- IKComponent
- IKComponent.Constraint
-  IKComponent.Constraint.DemandOptions 

Structure

# IKComponent.Constraint.DemandOptions

Flags for the different demands types that can be active in a single constraint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct DemandOptions
```

## Topics

### Initializers

init(rawValue: UInt)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt

The corresponding value of the raw type.

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

