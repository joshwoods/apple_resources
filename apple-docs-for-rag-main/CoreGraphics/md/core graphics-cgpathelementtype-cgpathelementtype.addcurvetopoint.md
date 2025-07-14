

- Core Graphics
- CGPathElementType
-  CGPathElementType.addCurveToPoint 

Case

# CGPathElementType.addCurveToPoint

The path element that adds a cubic curve from the current point to the specified point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case addCurveToPoint
```

## Discussion

The element holds two control points and a destination point. See the function CGPathAddCurveToPoint.

## See Also

### Constants

case moveToPoint

The path element that starts a new subpath.

case addLineToPoint

The path element that adds a line from the current point to a new point.

case addQuadCurveToPoint

The path element that adds a quadratic curve from the current point to the specified point.

case closeSubpath

The path element that closes and completes a subpath. The element does not contain any points. See the function closeSubpath().

