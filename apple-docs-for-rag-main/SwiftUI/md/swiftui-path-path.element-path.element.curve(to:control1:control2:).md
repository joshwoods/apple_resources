

- SwiftUI
- Path
- Path.Element
-  Path.Element.curve(to:control1:control2:) 

Case

# Path.Element.curve(to:control1:control2:)

A cubic Bézier curve from the previous current point to the given end-point, using the two control points to define the curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case curve(
    to: CGPoint,
    control1: CGPoint,
    control2: CGPoint
)
```

## Discussion

The end-point of the curve becomes the new current point.

## See Also

### Getting path elements

case closeSubpath

A line from the start point of the current subpath (if any) to the current point, which terminates the subpath.

case line(to: CGPoint)

A line from the previous current point to the given point, which becomes the new current point.

case move(to: CGPoint)

A path element that terminates the current subpath (without closing it) and defines a new current point.

case quadCurve(to: CGPoint, control: CGPoint)

A quadratic Bézier curve from the previous current point to the given end-point, using the single control point to define the curve.

