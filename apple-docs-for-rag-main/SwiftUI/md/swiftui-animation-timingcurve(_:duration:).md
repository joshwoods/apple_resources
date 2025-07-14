

- SwiftUI
- Animation
-  timingCurve(\_:duration:) 

Type Method

# timingCurve(\_:duration:)

Creates a new animation with speed controlled by the given curve.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func timingCurve(
    _ curve: UnitCurve,
    duration: TimeInterval
) -> Animation
```

## Parameters 

`duration`  

The duration of the animation, in seconds.

## See Also

### Creating custom animations

init&lt;A>(A)

Create an `Animation` that contains the specified custom animation.

static func timingCurve(Double, Double, Double, Double, duration: TimeInterval) -> Animation

An animation created from a cubic Bézier timing curve.

