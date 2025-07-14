

- UIKit
- UICubicTimingParameters
-  init(animationCurve:) 

Initializer

# init(animationCurve:)

Initializes the object with the specified UIKit timing curve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(animationCurve curve: UIView.AnimationCurve)
```

## Parameters 

`curve`  

The UIKit timing curve to use for the animations. You can specify a linear animation or an animation whose initial or final speed is slightly slower.

## Return Value

An initialized timing parameter object or `nil` if the object could not be created.

## Discussion

Use this method to create a timing curve that uses the standard UIKit timing curves such as UIView.AnimationCurve.easeIn, UIView.AnimationCurve.easeOut, UIView.AnimationCurve.easeInOut, or UIView.AnimationCurve.linear.

## See Also

### Initializing a cubic timing parameters object

init()

Initializes the object with the system’s default timing curve.

init(controlPoint1: CGPoint, controlPoint2: CGPoint)

Initializes the object with the specified control points for a cubic Bézier curve.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

