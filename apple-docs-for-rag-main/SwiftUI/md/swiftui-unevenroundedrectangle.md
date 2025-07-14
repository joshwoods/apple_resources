

- SwiftUI
-  UnevenRoundedRectangle 

Structure

# UnevenRoundedRectangle

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct UnevenRoundedRectangle
```

## Topics

### Creating an uneven rounded rectangle

init(cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle)

Creates a new rounded rectangle shape with uneven corners.

init(topLeadingRadius: CGFloat, bottomLeadingRadius: CGFloat, bottomTrailingRadius: CGFloat, topTrailingRadius: CGFloat, style: RoundedCornerStyle)

Creates a new rounded rectangle shape with uneven corners.

### Getting the shape’s characteristics

var cornerRadii: RectangleCornerRadii

The radii of each corner of the rounded rectangle.

var style: RoundedCornerStyle

The style of corners drawn by the rounded rectangle.

### Supporting types

var animatableData: RectangleCornerRadii.AnimatableData

The data to animate.

## Relationships

### Conforms To

- Animatable
- Copyable
- InsettableShape
- Sendable
- Shape
- View

## See Also

### Creating rectangular shapes

struct Rectangle

A rectangular shape aligned inside the frame of the view containing it.

struct RoundedRectangle

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

enum RoundedCornerStyle

Defines the shape of a rounded rectangle’s corners.

struct RectangleCornerRadii

Describes the corner radius values of a rounded rectangle with uneven corners.

