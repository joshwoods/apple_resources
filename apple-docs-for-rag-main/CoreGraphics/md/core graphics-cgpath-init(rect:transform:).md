

- Core Graphics
- CGPath
-  init(rect:transform:) 

Initializer

# init(rect:transform:)

Create an immutable path of a rectangle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    rect: CGRect,
    transform: UnsafePointer?
)
```

## Parameters 

`rect`  

The rectangle to add.

`transform`  

A pointer to an affine transformation matrix, or `NULL` if no transformation is needed. If specified, Core Graphics applies the transformation to the rectangle before it is added to the path.

## Return Value

A new, immutable path. You are responsible for releasing this object.

## Discussion

This is a convenience function that creates a path of an rectangle. Using this convenience function is more efficient than creating a mutable path and adding an rectangle to it.

Calling this function is equivalent to using CGRectGetMinX(_:) and related functions to find the corners of the rectangle, then using the CGPathMoveToPoint, CGPathAddLineToPoint, and closeSubpath() functions to draw the rectangle.

## See Also

### Creating Graphics Paths

init(ellipseIn: CGRect, transform: UnsafePointer&lt;CGAffineTransform>?)

Create an immutable path of an ellipse.

init(roundedRect: CGRect, cornerWidth: CGFloat, cornerHeight: CGFloat, transform: UnsafePointer&lt;CGAffineTransform>?)

Create an immutable path of a rounded rectangle.

