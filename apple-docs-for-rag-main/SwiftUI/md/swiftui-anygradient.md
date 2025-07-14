

- SwiftUI
-  AnyGradient 

Structure

# AnyGradient

A color gradient.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct AnyGradient
```

## Overview

When used as a ShapeStyle, this type draws a linear gradient with start-point \[0.5, 0\] and end-point \[0.5, 1\].

## Topics

### Creating a gradient

init(Gradient)

Creates a new instance from the specified gradient.

### Working with color spaces

func colorSpace(Gradient.ColorSpace) -> AnyGradient

Returns a version of the gradient that will use a specified color space for interpolating between its colors.

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

struct Gradient

A color gradient represented as an array of color stops, each having a parametric location value.

struct MeshGradient

A two-dimensional gradient defined by a 2D grid of positioned colors.

struct ShadowStyle

A style to use when rendering shadows.

