

- SwiftUI
-  RadialGradient 

Structure

# RadialGradient

A radial gradient.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct RadialGradient
```

## Overview

The gradient applies the color function as the distance from a center point, scaled to fit within the defined start and end radii. The gradient maps the unit space center point into the bounding rectangle of each shape filled with the gradient.

When using a radial gradient as a shape style, you can also use radialGradient(_:center:startRadius:endRadius:).

## Topics

### Creating a radial gradient

init(gradient: Gradient, center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat)

Creates a radial gradient from a base gradient.

init(colors: [Color], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat)

Creates a radial gradient from a collection of colors.

init(stops: [Gradient.Stop], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat)

Creates a radial gradient from a collection of color stops.

## Relationships

### Conforms To

- Sendable
- ShapeStyle
- View

## See Also

### Supporting types

struct AngularGradient

An angular gradient.

struct EllipticalGradient

A radial gradient that draws an ellipse.

struct LinearGradient

A linear gradient.

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

