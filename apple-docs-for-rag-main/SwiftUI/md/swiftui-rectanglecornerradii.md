

- SwiftUI
-  RectangleCornerRadii 

Structure

# RectangleCornerRadii

Describes the corner radius values of a rounded rectangle with uneven corners.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct RectangleCornerRadii
```

## Topics

### Creating a set of radii

init(topLeading: CGFloat, bottomLeading: CGFloat, bottomTrailing: CGFloat, topTrailing: CGFloat)

Creates a new set of corner radii for a rounded rectangle with uneven corners.

### Getting values for specific corners

var topLeading: CGFloat

The radius of the top-leading corner.

var topTrailing: CGFloat

The radius of the top-trailing corner.

var bottomLeading: CGFloat

The radius of the bottom-leading corner.

var bottomTrailing: CGFloat

The radius of the bottom-trailing corner.

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Creating rectangular shapes

struct Rectangle

A rectangular shape aligned inside the frame of the view containing it.

struct RoundedRectangle

A rectangular shape with rounded corners, aligned inside the frame of the view containing it.

enum RoundedCornerStyle

Defines the shape of a rounded rectangle’s corners.

struct UnevenRoundedRectangle

A rectangular shape with rounded corners with different values, aligned inside the frame of the view containing it.

