

- SwiftUI
- Shape
-  rect(topLeadingRadius:bottomLeadingRadius:bottomTrailingRadius:topTrailingRadius:style:) 

Type Method

# rect(topLeadingRadius:bottomLeadingRadius:bottomTrailingRadius:topTrailingRadius:style:)

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func rect(
    topLeadingRadius: CGFloat = 0,
    bottomLeadingRadius: CGFloat = 0,
    bottomTrailingRadius: CGFloat = 0,
    topTrailingRadius: CGFloat = 0,
    style: RoundedCornerStyle = .continuous
) -> Self
```

Available when `Self` is `UnevenRoundedRectangle`.

## See Also

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

