

- SwiftUI
-  AngularGradient 

Structure

# AngularGradient

An angular gradient.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct AngularGradient
```

## Overview

An angular gradient is also known as a “conic” gradient. This gradient applies the color function as the angle changes, relative to a center point and defined start and end angles. If `endAngle - startAngle > 2π`, the gradient only draws the last complete turn. If `endAngle - startAngle angularGradient(_:center:startAngle:endAngle:), conicGradient(_:center:angle:), or similar methods.

## Topics

### Creating a full rotation angular gradient

init(gradient: Gradient, center: UnitPoint, angle: Angle)

Creates a conic gradient that completes a full turn.

init(colors: [Color], center: UnitPoint, angle: Angle)

Creates a conic gradient from a collection of colors that completes a full turn.

init(stops: [Gradient.Stop], center: UnitPoint, angle: Angle)

Creates a conic gradient from a collection of color stops that completes a full turn.

### Creating a partial rotation angular gradient

init(gradient: Gradient, center: UnitPoint, startAngle: Angle, endAngle: Angle)

Creates an angular gradient.

init(colors: [Color], center: UnitPoint, startAngle: Angle, endAngle: Angle)

Creates an angular gradient from a collection of colors.

init(stops: [Gradient.Stop], center: UnitPoint, startAngle: Angle, endAngle: Angle)

Creates an angular gradient from a collection of color stops.

## Relationships

### Conforms To

- Sendable
- ShapeStyle
- View

## See Also

### Supporting types

struct EllipticalGradient

A radial gradient that draws an ellipse.

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

