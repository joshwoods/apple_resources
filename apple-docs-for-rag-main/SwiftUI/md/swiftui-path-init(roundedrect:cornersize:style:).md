

- SwiftUI
- Path
-  init(roundedRect:cornerSize:style:) 

Initializer

# init(roundedRect:cornerSize:style:)

Creates a path containing a rounded rectangle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    roundedRect rect: CGRect,
    cornerSize: CGSize,
    style: RoundedCornerStyle = .continuous
)
```

## Parameters 

`rect`  

A rectangle, specified in user space coordinates.

`cornerSize`  

The size of the corners, specified in user space coordinates.

`style`  

The corner style. Defaults to the `continous` style if not specified.

## Discussion

This is a convenience function that creates a path of a rounded rectangle. Using this convenience function is more efficient than creating a path and adding a rounded rectangle to it.

## See Also

### Creating a path

init()

Creates an empty path.

init(_:)

Creates an empty path, then executes a closure to add its initial elements.

init(ellipseIn: CGRect)

Creates a path as an ellipse within the given rectangle.

init(roundedRect: CGRect, cornerRadius: CGFloat, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

init(roundedRect: CGRect, cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle)

Creates a path as the given rounded rectangle, which may have uneven corner radii.

