

- SwiftUI
- Shape
-  rect 

Type Property

# rect

A rectangular shape aligned inside the frame of the view containing it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var rect: Rectangle { get }
```

Available when `Self` is `Rectangle`.

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

static func rect(cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

static func rect(cornerRadius: CGFloat, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

static func rect(cornerSize: CGSize, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

static func rect(topLeadingRadius: CGFloat, bottomLeadingRadius: CGFloat, bottomTrailingRadius: CGFloat, topTrailingRadius: CGFloat, style: RoundedCornerStyle) -> Self

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

