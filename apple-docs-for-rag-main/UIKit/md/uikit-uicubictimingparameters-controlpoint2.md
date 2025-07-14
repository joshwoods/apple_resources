

- UIKit
- UICubicTimingParameters
-  controlPoint2 

Instance Property

# controlPoint2

The second control point of the cubic Bézier curve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var controlPoint2: CGPoint { get }
```

## Discussion

This parameter contains the point you specified at initialization time. If you initialized the object with a UIView.AnimationCurve value instead, this property is set to CGPointZero.

## See Also

### Getting the timing parameters

var animationCurve: UIView.AnimationCurve

The standard UIKit animation curve to use for timing.

var controlPoint1: CGPoint

The first control point for the cubic Bézier curve.

