

- UIKit
- UIBezierPath
-  reversing() 

Instance Method

# reversing()

Creates and returns a new Bézier path object with the reversed contents of the current path.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func reversing() -> UIBezierPath
```

## Return Value

A new path object with the same path shape but for which the path has been created in the reverse direction.

## Discussion

Reversing a path does not necessarily change the appearance of the path when rendered. Instead, it changes the direction in which path segments are drawn. For example, reversing the path of a rectangle (whose line segments are normally drawn starting at the origin and proceeding in a counterclockwise direction) causes its line segments to be drawn in a clockwise direction instead. Drawing a reversed path could affect the appearance of a filled pattern, depending on the pattern and the fill rule in use.

This method reverses each whole or partial subpath in the path object individually.

## See Also

### Creating a Bézier path

convenience init(rect: CGRect)

Creates and returns a new Bézier path object with a rectangular path.

convenience init(ovalIn: CGRect)

Creates and returns a new Bézier path object with an inscribed oval path in the specified rectangle.

convenience init(roundedRect: CGRect, cornerRadius: CGFloat)

Creates and returns a new Bézier path object with a rounded rectangular path.

convenience init(roundedRect: CGRect, byRoundingCorners: UIRectCorner, cornerRadii: CGSize)

Creates and returns a new Bézier path object with a rectangular path rounded at the specified corners.

convenience init(arcCenter: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Creates and returns a new Bézier path object with an arc of a circle.

convenience init(cgPath: CGPath)

Creates and returns a new Bézier path object with the contents of a Core Graphics path.

init()

Creates and returns an empty path object.

init?(coder: NSCoder)

Creates a Bézier path object from data in an unarchiver.

