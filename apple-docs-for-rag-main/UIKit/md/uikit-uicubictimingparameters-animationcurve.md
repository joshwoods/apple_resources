

- UIKit
- UICubicTimingParameters
-  animationCurve 

Instance Property

# animationCurve

The standard UIKit animation curve to use for timing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var animationCurve: UIView.AnimationCurve { get }
```

## Discussion

If you initialized this object using an animation curve, this property reflects the curve you specified. If you initialized the object using the control points for a cubic Bézier curve, the value of this property is undefined.

## See Also

### Getting the timing parameters

var controlPoint1: CGPoint

The first control point for the cubic Bézier curve.

var controlPoint2: CGPoint

The second control point of the cubic Bézier curve.

