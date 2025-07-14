

- SwiftUI
-  InsettableShape 

Protocol

# InsettableShape

A shape type that is able to inset itself to produce another shape.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol InsettableShape : Shape
```

## Topics

### Setting the stroke border characteristics

func strokeBorder(_:lineWidth:antialiased:)

Returns a view that is the result of filling the `lineWidth`-sized border (aka inner stroke) of `self` with `content`. This is equivalent to insetting `self` by `lineWidth / 2` and stroking the resulting shape with `lineWidth` as the line-width.

func strokeBorder(lineWidth: CGFloat, antialiased: Bool) -> some View

Returns a view that is the result of filling the `lineWidth`-sized border (aka inner stroke) of `self` with the foreground color. This is equivalent to insetting `self` by `lineWidth / 2` and stroking the resulting shape with `lineWidth` as the line-width.

func strokeBorder(_:style:antialiased:)

Returns a view that is the result of insetting `self` by `style.lineWidth / 2`, stroking the resulting shape with `style`, and then filling with `content`.

func strokeBorder(style: StrokeStyle, antialiased: Bool) -> some View

Returns a view that is the result of insetting `self` by `style.lineWidth / 2`, stroking the resulting shape with `style`, and then filling with the foreground color.

### Setting the inset

func inset(by: CGFloat) -> Self.InsetShape

Returns `self` inset by `amount`.

**Required**

associatedtype InsetShape : InsettableShape

The type of the inset shape.

**Required**

## Relationships

### Inherits From

- Animatable
- Sendable
- Shape
- View

### Conforming Types

- ButtonBorderShape
- Capsule
- Circle
- ContainerRelativeShape
- Ellipse
- OffsetShape

  Conforms when `Content` conforms to `InsettableShape`.

- Rectangle
- RotatedShape

  Conforms when `Content` conforms to `InsettableShape`.

- RoundedRectangle
- UnevenRoundedRectangle

## See Also

### Setting a container shape

func containerShape&lt;T>(T) -> some View

Sets the container shape to use for any container relative shape within this view.

struct ContainerRelativeShape

A shape that is replaced by an inset version of the current container shape. If no container shape was defined, is replaced by a rectangle.

