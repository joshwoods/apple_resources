

- SwiftUI
-  RoundedRectangle 

Structure

# RoundedRectangle

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct RoundedRectangle
```

## Topics

### Creating a rounded rectangle

init(cornerRadius: CGFloat, style: RoundedCornerStyle)

Creates a new rounded rectangle shape.

init(cornerSize: CGSize, style: RoundedCornerStyle)

Creates a new rounded rectangle shape.

### Getting the shape’s characteristics

var cornerSize: CGSize

The width and height of the rounded rectangle’s corners.

var style: RoundedCornerStyle

The style of corners drawn by the rounded rectangle.

### Supporting types

var animatableData: CGSize.AnimatableData

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

enum RoundedCornerStyle

Defines the shape of a rounded rectangle’s corners.

struct UnevenRoundedRectangle

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

struct RectangleCornerRadii

Describes the corner radius values of a rounded rectangle with uneven corners.

