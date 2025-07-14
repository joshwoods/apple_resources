

- UIKit
-  UIRectEdge 

Structure

# UIRectEdge

Constants that specify the edges of a rectangle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
struct UIRectEdge
```

## Overview

You can add these constants together to specify multiple edges at the same time.

## Topics

### Edges

static var top: UIRectEdge

The top edge of the rectangle.

static var left: UIRectEdge

The left edge of the rectangle.

static var bottom: UIRectEdge

The bottom edge of the rectangle.

static var right: UIRectEdge

The right edge of the rectangle.

static var all: UIRectEdge

All edges of the rectangle.

### Initializers

init(rawValue: UInt)

Creates an edges structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Specifying the starting edges

var edges: UIRectEdge

The acceptable starting edges for the gesture.

