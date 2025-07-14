

- SpriteKit
-  SKActionTimingMode 

Enumeration

# SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum SKActionTimingMode
```

## Mentioned in 

Configuring Action Timing

## Topics

### Constants

case linear

Specifies linear pacing. Linear pacing causes an animation to occur evenly over its duration.

case easeIn

Specifies ease-in pacing. Ease-in pacing causes the animation to begin slowly and then speed up as it progresses.

case easeOut

Specifies ease-out pacing. Ease-out pacing causes the animation to begin quickly and then slow as it completes.

case easeInEaseOut

Specifies ease-in ease-out pacing. An ease-in ease-out animation begins slowly, accelerates through the middle of its duration, and then slows again before completing.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var duration: TimeInterval

The duration required to complete an action.

var timingMode: SKActionTimingMode

A setting that controls the speed curve of an animation.

var timingFunction: SKActionTimingFunction

A block used to customize the timing function.

typealias SKActionTimingFunction

The signature for the custom timing block.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

