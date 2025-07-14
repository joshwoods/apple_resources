

- SpriteKit
- SKAction
-  timingFunction 

Instance Property

# timingFunction

A block used to customize the timing function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var timingFunction: SKActionTimingFunction { get set }
```

## Mentioned in 

Getting Started with Actions

Configuring Action Timing

## Discussion

If a timing function is provided, after the normal timing mode is applied, the result is sent to the timing function. The return SKActionTimingFunction value of the timing function determines the actual time used to perform the animation.

The following code shows how you can create a custom timing function using simd_smoothstep(_:_:_:) interpolation:

```
import simd
let horizontalAction = SKAction.moveTo(x: end.x, duration: 2.0)
horizontalAction.timingFunction = {
    time in
    return simd_smoothstep(0, 1, time)
}
```

If the above code is combined with a vertical linear move action, the path taken by a node running this action describes the curve illustrated below:

## See Also

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var duration: TimeInterval

The duration required to complete an action.

var timingMode: SKActionTimingMode

A setting that controls the speed curve of an animation.

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

typealias SKActionTimingFunction

The signature for the custom timing block.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

