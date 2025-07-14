

- SwiftUI
- Shape
-  buttonBorder 

Type Property

# buttonBorder

A shape that defers to the environment to determine the resolved button border shape.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var buttonBorder: ButtonBorderShape { get }
```

Available when `Self` is `ButtonBorderShape`.

## Discussion

You can override the resolved shape in a given view hierarchy by using the buttonBorderShape(_:) modifier. If no button border shape is specified, it is resolved automatically for the given context and platform.

## See Also

### Getting standard shapes

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

