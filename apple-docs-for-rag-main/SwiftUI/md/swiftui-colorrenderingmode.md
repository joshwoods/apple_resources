

- SwiftUI
-  ColorRenderingMode 

Enumeration

# ColorRenderingMode

The set of possible working color spaces for color-compositing operations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum ColorRenderingMode
```

## Overview

Each color space guarantees the preservation of a particular range of color values.

## Topics

### Getting rendering modes

case extendedLinear

The extended linear sRGB working color space.

case linear

The linear sRGB working color space.

case nonLinear

The non-linear sRGB working color space.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Compositing views

func blendMode(BlendMode) -> some View

Sets the blend mode for compositing this view with overlapping views.

func compositingGroup() -> some View

Wraps this view in a compositing group.

func drawingGroup(opaque: Bool, colorMode: ColorRenderingMode) -> some View

Composites this view’s contents into an offscreen image before final display.

enum BlendMode

Modes for compositing a view with overlapping content.

