

- SwiftUI
-  StrokeBorderShapeView 

Structure

# StrokeBorderShapeView

A shape provider that strokes the border of its shape.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct StrokeBorderShapeView where Content : InsettableShape, Style : ShapeStyle, Background : View
```

## Overview

You don’t create this type directly; it’s the return type of `Shape.strokeBorder`.

## Topics

### Creating a stroke border shape view

init(shape: Content, style: Style, strokeStyle: StrokeStyle, isAntialiased: Bool, background: Background)

Create a stroke border shape.

### Getting shape view properties

var background: Background

The background shown beneath this view.

var isAntialiased: Bool

Whether this shape should be drawn antialiased.

var shape: Content

The shape that this type draws and provides for other drawing operations.

var strokeStyle: StrokeStyle

The stroke style used when stroking this view’s shape.

var style: Style

The style that strokes the border of this view’s shape.

## Relationships

### Conforms To

- ShapeView
- View

## See Also

### Defining shape behavior

protocol ShapeView

A view that provides a shape that you can use for drawing operations.

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

struct FillStyle

A style for rasterizing vector shapes.

struct FillShapeView

A shape provider that fills its shape.

