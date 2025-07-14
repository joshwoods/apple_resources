

- SpriteKit
- SKActionTimingMode
-  SKActionTimingMode.easeInEaseOut 

Case

# SKActionTimingMode.easeInEaseOut

Specifies ease-in ease-out pacing. An ease-in ease-out animation begins slowly, accelerates through the middle of its duration, and then slows again before completing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case easeInEaseOut
```

## Discussion

By creating two separate actions, a moveTo(x:duration:) and a moveTo(y:duration:), and setting the former to SKActionTimingMode.easeInEaseOut, you can visualize the effect of this timing mode by tracing the path of a circular shape node running the actions in a group:

## See Also

### Constants

case linear

Specifies linear pacing. Linear pacing causes an animation to occur evenly over its duration.

case easeIn

Specifies ease-in pacing. Ease-in pacing causes the animation to begin slowly and then speed up as it progresses.

case easeOut

Specifies ease-out pacing. Ease-out pacing causes the animation to begin quickly and then slow as it completes.

