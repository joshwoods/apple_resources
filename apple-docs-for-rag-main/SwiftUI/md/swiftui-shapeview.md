

- SwiftUI
-  ShapeView 

Protocol

# ShapeView

A view that provides a shape that you can use for drawing operations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol ShapeView : View
```

## Overview

Use this type with the drawing methods on Shape to apply multiple fills and/or strokes to a shape. For example, the following code applies a fill and stroke to a capsule shape:

```
Capsule()
    .fill(.yellow)
    .stroke(.blue, lineWidth: 8)
```

## Topics

### Getting the shape

var shape: Self.Content

The shape that this type draws and provides for other drawing operations.

**Required**

associatedtype Content : Shape

The type of shape this can provide.

**Required**

### Modify the shape

func fill&lt;S>(S, style: FillStyle) -> FillShapeView&lt;Self.Content, S, Self>

Fills this shape with a color or gradient.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self.Content, S, Self>

Traces the outline of this shape with a color or gradient.

func strokeBorder&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of insetting this view by half of its style’s line width.

func strokeBorder&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeBorderShapeView&lt;Self.Content, S, Self>

Returns a view that’s the result of filling an inner stroke of this view with the content you supply.

## Relationships

### Inherits From

- View

### Conforming Types

- FillShapeView
- StrokeBorderShapeView
- StrokeShapeView

## See Also

### Defining shape behavior

protocol Shape

A 2D shape that you can use when drawing a view.

struct AnyShape

A type-erased shape value.

enum ShapeRole

Ways of styling a shape.

struct StrokeStyle

The characteristics of a stroke that traces a path.

struct StrokeShapeView

A shape provider that strokes its shape.

struct StrokeBorderShapeView

A shape provider that strokes the border of its shape.

struct FillStyle

A style for rasterizing vector shapes.

struct FillShapeView

A shape provider that fills its shape.

