

- SwiftUI
-  EllipticalGradient 

Structure

# EllipticalGradient

A radial gradient that draws an ellipse.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct EllipticalGradient
```

## Overview

The gradient maps its coordinate space to the unit space square in which its center and radii are defined, then stretches that square to fill its bounding rect, possibly also stretching the circular gradient to have elliptical contours.

For example, an elliptical gradient centered on the view, filling its bounds:

```
EllipticalGradient(gradient: .init(colors: [.red, .yellow]))
```

When using an elliptical gradient as a shape style, you can also use ellipticalGradient(_:center:startRadiusFraction:endRadiusFraction:).

## Topics

### Creating an elliptical gradient

init(gradient: Gradient, center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat)

Creates an elliptical gradient.

init(colors: [Color], center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat)

Creates an elliptical gradient from a collection of colors.

init(stops: [Gradient.Stop], center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat)

Creates an elliptical gradient from a collection of color stops.

## Relationships

### Conforms To

- Sendable
- ShapeStyle
- View

## See Also

### Supporting types

struct AngularGradient

An angular gradient.

struct LinearGradient

A linear gradient.

struct RadialGradient

A radial gradient.

struct Material

A background material type.

struct ImagePaint

A shape style that fills a shape by repeating a region of an image.

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

