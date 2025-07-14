

- UIKit
- UIBezierPath
-  init(cgPath:) 

Initializer

# init(cgPath:)

Creates and returns a new Bézier path object with the contents of a Core Graphics path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(cgPath CGPath: CGPath)
```

## Parameters 

`CGPath`  

The Core Graphics path from which to obtain the initial path information. If this parameter is `nil`, the method raises an exception.

## Return Value

A new path object with the specified path information.

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

func reversing() -> UIBezierPath

Creates and returns a new Bézier path object with the reversed contents of the current path.

init()

Creates and returns an empty path object.

init?(coder: NSCoder)

Creates a Bézier path object from data in an unarchiver.

