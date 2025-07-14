

- SwiftUI
-  Shape 

Protocol

# Shape

A 2D shape that you can use when drawing a view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Shape : Sendable, Animatable, View, _RemoveGlobalActorIsolation
```

## Overview

Shapes without an explicit fill or stroke get a default fill based on the foreground color.

You can define shapes in relation to an implicit frame of reference, such as the natural size of the view that contains it. Alternatively, you can define shapes in terms of absolute coordinates.

## Topics

### Getting standard shapes

static var buttonBorder: ButtonBorderShape

A shape that defers to the environment to determine the resolved button border shape.

static var capsule: Capsule

A capsule shape aligned inside the frame of the view containing it.

static func capsule(style: RoundedCornerStyle) -> Self

A capsule shape aligned inside the frame of the view containing it.

static var circle: Circle

A circle centered on the frame of the view containing it.

static var containerRelative: ContainerRelativeShape

A shape that is replaced by an inset version of the current container shape. If no container shape was defined, is replaced by a rectangle.

static var ellipse: Ellipse

An ellipse aligned inside the frame of the view containing it.

static var rect: Rectangle

A rectangular shape aligned inside the frame of the view containing it.

static func rect(cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

static func rect(cornerRadius: CGFloat, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

static func rect(cornerSize: CGSize, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

static func rect(topLeadingRadius: CGFloat, bottomLeadingRadius: CGFloat, bottomTrailingRadius: CGFloat, topTrailingRadius: CGFloat, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

### Defining a shape’s size and path

func sizeThatFits(ProposedViewSize) -> CGSize

Returns the size of the view that will render the shape, given a proposed size.

**Required** Default implementation provided.

func path(in: CGRect) -> Path

Describes this shape as a path within a rectangular frame of reference.

**Required**

### Transforming a shape

func trim(from: CGFloat, to: CGFloat) -> some Shape

Trims this shape by a fractional amount based on its representation as a path.

func transform(CGAffineTransform) -> TransformedShape&lt;Self>

Applies an affine transform to this shape.

func size(CGSize) -> some Shape

Returns a new version of self representing the same shape, but that will ask it to create its path from a rect of `size`. This does not affect the layout properties of any views created from the shape (e.g. by filling it).

func size(width: CGFloat, height: CGFloat) -> some Shape

Returns a new version of self representing the same shape, but that will ask it to create its path from a rect of size `(width, height)`. This does not affect the layout properties of any views created from the shape (e.g. by filling it).

func scale(CGFloat, anchor: UnitPoint) -> ScaledShape&lt;Self>

Scales this shape without changing its bounding frame.

func scale(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> ScaledShape&lt;Self>

Scales this shape without changing its bounding frame.

func rotation(Angle, anchor: UnitPoint) -> RotatedShape&lt;Self>

Rotates this shape around an anchor point at the angle you specify.

func offset(_:)

Changes the relative position of this shape using the specified point.

func offset(x: CGFloat, y: CGFloat) -> OffsetShape&lt;Self>

Changes the relative position of this shape using the specified point.

### Setting the stroke characteristics

func stroke&lt;S>(S, lineWidth: CGFloat) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, lineWidth: CGFloat, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(lineWidth: CGFloat) -> some Shape

Returns a new shape that is a stroked copy of `self` with line-width defined by `lineWidth` and all other properties of `StrokeStyle` having their default values.

func stroke&lt;S>(S, style: StrokeStyle) -> some View

Traces the outline of this shape with a color or gradient.

func stroke&lt;S>(S, style: StrokeStyle, antialiased: Bool) -> StrokeShapeView&lt;Self, S, EmptyView>

Traces the outline of this shape with a color or gradient.

func stroke(style: StrokeStyle) -> some Shape

Returns a new shape that is a stroked copy of `self`, using the contents of `style` to define the stroke characteristics.

### Filling a shape

func fill(_:style:)

Fills this shape with a color or gradient.

func fill(style: FillStyle) -> some View

Fills this shape with the foreground color.

### Setting the role

static var role: ShapeRole

An indication of how to style a shape.

**Required** Default implementation provided.

### Indicating a layout direction

var layoutDirectionBehavior: LayoutDirectionBehavior

Returns the behavior this shape should use for different layout directions.

**Required** Default implementation provided.

### Performing operations on a shape

func intersection&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions common to both shapes.

func lineIntersection&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with a line from this shape that overlaps the filled regions of the given shape.

func lineSubtraction&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with a line from this shape that does not overlap the filled region of the given shape.

func subtracting&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions from this shape that are not in the given shape.

func symmetricDifference&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions either from this shape or the given shape, but not in both.

func union&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions in either this shape or the given shape.

### Instance Methods

func size(CGSize, anchor: UnitPoint) -> some Shape

Returns a new version of self representing the same shape, but within a rect of `size` instead of the container size.

func size(width: CGFloat, height: CGFloat, anchor: UnitPoint) -> some Shape

Returns a new version of self representing the same shape, but within a rect of `(width, height)` instead of the container size.

## Relationships

### Inherits From

- Animatable
- Sendable
- View

### Inherited By

- InsettableShape

### Conforming Types

- AnyShape
- ButtonBorderShape
- Capsule
- Circle
- ContainerRelativeShape
- Ellipse
- OffsetShape

  Conforms when `Content` conforms to `InsettableShape`.

- Path
- Rectangle
- RotatedShape
- RoundedRectangle
- ScaledShape
- TransformedShape
- UnevenRoundedRectangle

## See Also

### Defining shape behavior

protocol ShapeView

A view that provides a shape that you can use for drawing operations.

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

