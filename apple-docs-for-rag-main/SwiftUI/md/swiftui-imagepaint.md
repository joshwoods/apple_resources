

- SwiftUI
-  ImagePaint 

Structure

# ImagePaint

A shape style that fills a shape by repeating a region of an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct ImagePaint
```

## Overview

You can also use image(_:sourceRect:scale:) to construct this style.

## Topics

### Creating an image paint style

init(image: Image, sourceRect: CGRect, scale: CGFloat)

Creates a shape-filling shape style.

### Configuring the image paint style

var image: Image

The image to be drawn.

var scale: CGFloat

A scale factor applied to the image while being drawn.

var sourceRect: CGRect

A unit-space rectangle defining how much of the source image to draw.

## Relationships

### Conforms To

- Sendable
- ShapeStyle

## See Also

### Supporting types

struct AngularGradient

An angular gradient.

struct EllipticalGradient

A radial gradient that draws an ellipse.

struct LinearGradient

A linear gradient.

struct RadialGradient

A radial gradient.

struct Material

A background material type.

struct HierarchicalShapeStyle

A shape style that maps to one of the numbered content styles.

struct HierarchicalShapeStyleModifier

Styles that you can apply to hierarchical shapes.

struct ForegroundStyle

The foreground style in the current context.

struct BackgroundStyle

The background style in the current context.

struct SelectionShapeStyle

A style used to visually indicate selection following platform conventional colors and behaviors.

struct SeparatorShapeStyle

A style appropriate for foreground separator or border lines.

struct TintShapeStyle

A style that reflects the current tint color.

struct FillShapeStyle

A shape style that displays one of the overlay fills.

struct LinkShapeStyle

A style appropriate for links.

struct PlaceholderTextShapeStyle

A style appropriate for placeholder text.

