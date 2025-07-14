

- SwiftUI
-  Gradient 

Structure

# Gradient

A color gradient represented as an array of color stops, each having a parametric location value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Gradient
```

## Mentioned in 

Adding a background to your view

## Topics

### Creating a gradient from colors

init(colors: [Color])

Creates a gradient from an array of colors.

### Creating a gradient from stops

init(stops: [Gradient.Stop])

Creates a gradient from an array of color stops.

var stops: [Gradient.Stop]

The array of color stops.

struct Stop

One color stop in the gradient.

### Working with color spaces

func colorSpace(Gradient.ColorSpace) -> AnyGradient

Returns a version of the gradient that will use a specified color space for interpolating between its colors.

struct ColorSpace

A method of interpolating between the colors in a gradient.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- ScaleRange
- Sendable
- ShapeStyle

## See Also

### Styling content

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

var backgroundStyle: AnyShapeStyle?

An optional style that overrides the default system background style when set.

protocol ShapeStyle

A color or pattern to use when rendering a shape.

struct AnyShapeStyle

A type-erased ShapeStyle value.

struct MeshGradient

A two-dimensional gradient defined by a 2D grid of positioned colors.

struct AnyGradient

A color gradient.

struct ShadowStyle

A style to use when rendering shadows.

