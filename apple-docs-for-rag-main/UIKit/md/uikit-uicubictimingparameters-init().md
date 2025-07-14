

- UIKit
- UICubicTimingParameters
-  init() 

Initializer

# init()

Initializes the object with the system’s default timing curve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init()
```

## Return Value

An initialized timing parameter object or `nil` if the object could not be created.

## Discussion

Use this method to create a timing curve based on the default Core Animation timing function.

## See Also

### Initializing a cubic timing parameters object

init(animationCurve: UIView.AnimationCurve)

Initializes the object with the specified UIKit timing curve.

init(controlPoint1: CGPoint, controlPoint2: CGPoint)

Initializes the object with the specified control points for a cubic Bézier curve.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

