

- SwiftUI
- Path
-  init(\_:) 

Initializer

# init(\_:)

Creates an empty path, then executes a closure to add its initial elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ callback: (inout Path) -> ())
```

Show all declarations

## Parameters 

`callback`  

The Swift function that will be called to initialize the new path.

## See Also

### Creating a path

init()

Creates an empty path.

init(ellipseIn: CGRect)

Creates a path as an ellipse within the given rectangle.

init(roundedRect: CGRect, cornerRadius: CGFloat, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

init(roundedRect: CGRect, cornerSize: CGSize, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

init(roundedRect: CGRect, cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle)

Creates a path as the given rounded rectangle, which may have uneven corner radii.

