

- SwiftUI
-  StrokeStyle 

Structure

# StrokeStyle

The characteristics of a stroke that traces a path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct StrokeStyle
```

## Topics

### Creating a stroke style

init(lineWidth: CGFloat, lineCap: CGLineCap, lineJoin: CGLineJoin, miterLimit: CGFloat, dash: [CGFloat], dashPhase: CGFloat)

Creates a new stroke style from the given components.

### Setting stroke style properties

var lineWidth: CGFloat

The width of the stroked path.

var lineCap: CGLineCap

The endpoint style of a line.

var lineJoin: CGLineJoin

The join type of a line.

var miterLimit: CGFloat

A threshold used to determine whether to use a bevel instead of a miter at a join.

var dash: [CGFloat]

The lengths of painted and unpainted segments used to make a dashed line.

var dashPhase: CGFloat

How far into the dash pattern the line starts.

## Relationships

### Conforms To

- Animatable
- Copyable
- Equatable
- Sendable

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

struct StrokeShapeView

A shape provider that strokes its shape.

struct StrokeBorderShapeView

A shape provider that strokes the border of its shape.

struct FillStyle

A style for rasterizing vector shapes.

struct FillShapeView

A shape provider that fills its shape.

