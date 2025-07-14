

- SwiftUI
-  FillShapeView 

Structure

# FillShapeView

A shape provider that fills its shape.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct FillShapeView where Content : Shape, Style : ShapeStyle, Background : View
```

## Overview

You do not create this type directly, it is the return type of `Shape.fill`.

## Topics

### Creating a stroke shape view

init(shape: Content, style: Style, fillStyle: FillStyle, background: Background)

Create a FillShapeView.

### Getting shape view properties

var background: Background

The background shown beneath this view.

var fillStyle: FillStyle

The fill style used when filling this view’s shape.

var shape: Content

The shape that this type draws and provides for other drawing operations.

var style: Style

The style that fills this view’s shape.

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

struct StrokeBorderShapeView

A shape provider that strokes the border of its shape.

struct FillStyle

A style for rasterizing vector shapes.

