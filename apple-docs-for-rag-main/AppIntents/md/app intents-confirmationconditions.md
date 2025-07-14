

- App Intents
-  ConfirmationConditions 

Structure

# ConfirmationConditions

Conditions for a confirmation request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ConfirmationConditions
```

## Overview

If any of the conditions are met, confirmation will be requested.

## Topics

### Initializers

init(rawValue: Int)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let lowConfidenceSource: ConfirmationConditions

Only confirm if initiated from a low-confidence action source.

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
- Sendable
- SetAlgebra

