

- AppKit
- NSGradient
-  NSGradient.DrawingOptions 

Structure

# NSGradient.DrawingOptions

Constants that specify gradient drawing options.

macOS

``` source
struct DrawingOptions
```

## Overview

These constants are used by the primitive drawing methods to determine if drawing occurs outside of the gradient start and end locations.

## Topics

### Constants

static var drawsBeforeStartingLocation: NSGradient.DrawingOptions

Drawing extends before the gradient starting point.

static var drawsAfterEndingLocation: NSGradient.DrawingOptions

Drawing extends beyond the gradient end point.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

