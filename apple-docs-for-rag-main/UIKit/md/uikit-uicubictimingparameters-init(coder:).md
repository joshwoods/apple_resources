

- UIKit
- UICubicTimingParameters
-  init(coder:) 

Initializer

# init(coder:)

Creates a timing parameters object from data in an unarchiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Initializing a cubic timing parameters object

init()

Initializes the object with the system’s default timing curve.

init(animationCurve: UIView.AnimationCurve)

Initializes the object with the specified UIKit timing curve.

init(controlPoint1: CGPoint, controlPoint2: CGPoint)

Initializes the object with the specified control points for a cubic Bézier curve.

