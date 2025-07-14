

- SwiftUI
-  FillStyle 

Structure

# FillStyle

A style for rasterizing vector shapes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct FillStyle
```

## Topics

### Creating a fill style

init(eoFill: Bool, antialiased: Bool)

Creates a new fill style with the specified settings.

### Setting fill style properties

var isEOFilled: Bool

A Boolean value that indicates whether to use the even-odd rule when rendering a shape.

var isAntialiased: Bool

A Boolean value that indicates whether to apply antialiasing to the edges of a shape.

## Relationships

### Conforms To

- BitwiseCopyable
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

struct StrokeStyle

The characteristics of a stroke that traces a path.

struct StrokeShapeView

A shape provider that strokes its shape.

struct StrokeBorderShapeView

A shape provider that strokes the border of its shape.

struct FillShapeView

A shape provider that fills its shape.

