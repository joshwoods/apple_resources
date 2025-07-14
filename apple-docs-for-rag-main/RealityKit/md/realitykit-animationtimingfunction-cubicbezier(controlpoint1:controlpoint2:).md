

- RealityKit
- AnimationTimingFunction
-  cubicBezier(controlPoint1:controlPoint2:) 

Type Method

# cubicBezier(controlPoint1:controlPoint2:)

Creates a timing function that accelerates and then decelerates towards the target value with the cubic bezier shape specified by two control points.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static func cubicBezier(
    controlPoint1: SIMD2,
    controlPoint2: SIMD2
) -> AnimationTimingFunction
```

## Parameters 

`controlPoint1`  

The first control point for the cubic bezier function.

`controlPoint2`  

The second control point for the cubic bezier function.

## Return Value

The cubic bezier timing function.

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

static var linear: AnimationTimingFunction

A timing function that produces a linear transition.

