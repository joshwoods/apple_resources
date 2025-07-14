

- SwiftUI
- Path
-  addRoundedRect(in:cornerRadii:style:transform:) 

Instance Method

# addRoundedRect(in:cornerRadii:style:transform:)

Adds a rounded rectangle with uneven corners to the path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func addRoundedRect(
    in rect: CGRect,
    cornerRadii: RectangleCornerRadii,
    style: RoundedCornerStyle = .continuous,
    transform: CGAffineTransform = .identity
)
```

## Parameters 

`rect`  

A rectangle, specified in user space coordinates.

`cornerRadii`  

The radius of each corner of the rectangle, specified in user space coordinates.

`style`  

The corner style. Defaults to the `continous` style if not specified.

`transform`  

An affine transform to apply to the rectangle before adding to the path. Defaults to the identity transform if not specified.

## Discussion

This is a convenience function that adds a rounded rectangle to a path, starting by moving to the center of the right edge and then adding lines and curves counter-clockwise to create a rounded rectangle, closing the subpath.

