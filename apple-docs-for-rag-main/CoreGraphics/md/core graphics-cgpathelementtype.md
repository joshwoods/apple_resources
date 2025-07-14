

- Core Graphics
-  CGPathElementType 

Enumeration

# CGPathElementType

The type of element found in a path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGPathElementType
```

## Overview

For more information about paths, see CGPath.

## Topics

### Constants

case moveToPoint

The path element that starts a new subpath.

case addLineToPoint

The path element that adds a line from the current point to a new point.

case addQuadCurveToPoint

The path element that adds a quadratic curve from the current point to the specified point.

case addCurveToPoint

The path element that adds a cubic curve from the current point to the specified point.

case closeSubpath

The path element that closes and completes a subpath. The element does not contain any points. See the function closeSubpath().

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Applying a Function to the Elements of a Path

func apply(info: UnsafeMutableRawPointer?, function: CGPathApplierFunction)

For each element in a graphics path, calls a custom applier function.

typealias CGPathApplierFunction

Defines a callback function that can view an element in a graphics path.

struct CGPathElement

A data structure that provides information about a path element.

