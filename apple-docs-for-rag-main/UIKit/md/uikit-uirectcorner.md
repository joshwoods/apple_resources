

- UIKit
-  UIRectCorner 

Structure

# UIRectCorner

The corners of a rectangle.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
struct UIRectCorner
```

## Overview

The specified constants reflect the corners of a rectangle that has not been modified by an affine transform and is drawn in the default coordinate system (where the origin is in the upper-left corner and positive values extend down and to the right).

## Topics

### Constants

static var topLeft: UIRectCorner

The top-left corner of the rectangle.

static var topRight: UIRectCorner

The top-right corner of the rectangle.

static var bottomLeft: UIRectCorner

The bottom-left corner of the rectangle.

static var bottomRight: UIRectCorner

The bottom-right corner of the rectangle.

static var allCorners: UIRectCorner

All corners of the rectangle.

### Initializer

init(rawValue: UInt)

Creates a structure that represents the corners of a rectangle.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

