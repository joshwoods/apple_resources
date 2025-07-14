

- UIKit
- UIBezierPath
-  init(ovalIn:) 

Initializer

# init(ovalIn:)

Creates and returns a new Bézier path object with an inscribed oval path in the specified rectangle.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(ovalIn rect: CGRect)
```

## Parameters 

`rect`  

The rectangle in which to inscribe an oval.

## Return Value

A new path object with the oval path.

## Discussion

This method creates a closed subpath that approximates the oval using a sequence of Bézier curves. The path is created in a clockwise direction (relative to the default coordinate system). If the `rect` parameter specifies a square, the inscribed path is a circle.

## See Also

### Creating a Bézier path

convenience init(rect: CGRect)

Creates and returns a new Bézier path object with a rectangular path.

convenience init(roundedRect: CGRect, cornerRadius: CGFloat)

Creates and returns a new Bézier path object with a rounded rectangular path.

convenience init(roundedRect: CGRect, byRoundingCorners: UIRectCorner, cornerRadii: CGSize)

Creates and returns a new Bézier path object with a rectangular path rounded at the specified corners.

convenience init(arcCenter: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Creates and returns a new Bézier path object with an arc of a circle.

convenience init(cgPath: CGPath)

Creates and returns a new Bézier path object with the contents of a Core Graphics path.

func reversing() -> UIBezierPath

Creates and returns a new Bézier path object with the reversed contents of the current path.

init()

Creates and returns an empty path object.

init?(coder: NSCoder)

Creates a Bézier path object from data in an unarchiver.

