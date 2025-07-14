

- SwiftUI
- Path
-  init(roundedRect:cornerRadii:style:) 

Initializer

# init(roundedRect:cornerRadii:style:)

Creates a path as the given rounded rectangle, which may have uneven corner radii.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    roundedRect rect: CGRect,
    cornerRadii: RectangleCornerRadii,
    style: RoundedCornerStyle = .continuous
)
```

## Parameters 

`rect`  

A rectangle, specified in user space coordinates.

`cornerRadii`  

The radius of each corner of the rectangle, specified in user space coordinates.

`style`  

The corner style. Defaults to the `continous` style if not specified.

## Discussion

This is a convenience function that creates a path of a rounded rectangle. Using this function is more efficient than creating a path and adding a rounded rectangle to it.

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

init(roundedRect: CGRect, cornerSize: CGSize, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

