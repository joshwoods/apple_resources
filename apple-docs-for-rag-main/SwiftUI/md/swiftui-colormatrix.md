

- SwiftUI
-  ColorMatrix 

Structure

# ColorMatrix

A matrix to use in an RGBA color transformation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct ColorMatrix
```

## Overview

The matrix has five columns, each with a red, green, blue, and alpha component. You can use the matrix for tasks like creating a color transformation GraphicsContext.Filter for a GraphicsContext using the colorMatrix(_:) method.

## Topics

### Creating an identity matrix

init()

Creates the identity matrix.

### First column

var r1: Float

var g1: Float

var b1: Float

var a1: Float

### Second column

var r2: Float

var g2: Float

var b2: Float

var a2: Float

### Third column

var r3: Float

var g3: Float

var b3: Float

var a3: Float

### Fourth column

var r4: Float

var g4: Float

var b4: Float

var a4: Float

### Fifth column

var r5: Float

var g5: Float

var b5: Float

var a5: Float

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Applying blur and shadows

func blur(radius: CGFloat, opaque: Bool) -> some View

Applies a Gaussian blur to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

