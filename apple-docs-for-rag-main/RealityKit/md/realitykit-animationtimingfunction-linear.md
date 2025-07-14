

- RealityKit
- AnimationTimingFunction
-  linear 

Type Property

# linear

A timing function that produces a linear transition.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static var linear: AnimationTimingFunction { get }
```

## See Also

### Creating timing functions

static var `default`: AnimationTimingFunction

A timing function that produces the default curve for the transition.

static var easeIn: AnimationTimingFunction

A timing function that produces a gradual starting transition.

static var easeInOut: AnimationTimingFunction

A timing function that produces a gradual starting and ending transition.

static var easeOut: AnimationTimingFunction

A timing function that produces a gradual ending transition.

static func cubicBezier(controlPoint1: SIMD2&lt;Float>, controlPoint2: SIMD2&lt;Float>) -> AnimationTimingFunction

Creates a timing function that accelerates and then decelerates towards the target value with the cubic bezier shape specified by two control points.

