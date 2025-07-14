

- SwiftUI
- Animation
-  init(\_:) 

Initializer

# init(\_:)

Create an `Animation` that contains the specified custom animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(_ base: A) where A : CustomAnimation
```

## See Also

### Creating custom animations

static func timingCurve(UnitCurve, duration: TimeInterval) -> Animation

Creates a new animation with speed controlled by the given curve.

static func timingCurve(Double, Double, Double, Double, duration: TimeInterval) -> Animation

An animation created from a cubic Bézier timing curve.

