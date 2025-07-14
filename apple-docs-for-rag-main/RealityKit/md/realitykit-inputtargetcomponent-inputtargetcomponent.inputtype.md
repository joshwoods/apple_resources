

- RealityKit
- InputTargetComponent
-  InputTargetComponent.InputType 

Structure

# InputTargetComponent.InputType

A type of input that the `InputTargetComponent`’s entity can receive.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct InputType
```

## Topics

### Initializers

init(rawValue: UInt32)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt32

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let all: InputTargetComponent.InputType

All forms of input.

static let direct: InputTargetComponent.InputType

All forms of input that target content by querying proximity from the input device to the content.

static let indirect: InputTargetComponent.InputType

All forms of input that target content using an indirect targeting mechanism.

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

