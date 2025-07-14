

- RealityKit
- PortalComponent
-  PortalComponent.Options 

Structure

# PortalComponent.Options

Options to toggle the portal features on and off.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Options
```

## Overview

This option set is equivalent to setting clippingMode and crossingMode directly.

Use this type with init(target:plane:options:).

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

### Type Properties

static let allowCrossing: PortalComponent.Options

An option that enables the crossing feature.

static let clipContents: PortalComponent.Options

An option that enables the clipping feature.

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

