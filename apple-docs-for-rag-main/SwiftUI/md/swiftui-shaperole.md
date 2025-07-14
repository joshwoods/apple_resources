

- SwiftUI
-  ShapeRole 

Enumeration

# ShapeRole

Ways of styling a shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ShapeRole
```

## Topics

### Getting shape roles

case fill

Indicates to the shape’s style that SwiftUI fills the shape.

case stroke

Indicates to the shape’s style that SwiftUI applies a stroke to the shape’s path.

case separator

Indicates to the shape’s style that SwiftUI uses the shape as a separator.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Defining shape behavior

protocol ShapeView

A view that provides a shape that you can use for drawing operations.

protocol Shape

A 2D shape that you can use when drawing a view.

struct AnyShape

A type-erased shape value.

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

