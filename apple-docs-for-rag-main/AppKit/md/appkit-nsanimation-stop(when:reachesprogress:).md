

- AppKit
- NSAnimation
-  stop(when:reachesProgress:) 

Instance Method

# stop(when:reachesProgress:)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

macOS

``` source
func stop(
    when animation: NSAnimation,
    reachesProgress stopProgress: NSAnimation.Progress
)
```

## Parameters 

`animation`  

The other `NSAnimation` object with which the receiver is linked.

`stopProgress`  

A `float` value (typed as NSAnimationProgress) that specifies a progress mark of the other animation.

## Discussion

This method links the running of two animations together. You can set only one `NSAnimation` object as a start animation and one as a stop animation at any one time. Setting a new stop animation removes any animation previously set.

## See Also

### Related Documentation

func stop()

Stops the animation represented by the receiver.

### Linking Animations Together

func start(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

func clearStart()

Clears linkage to another animation that causes the receiver to start.

func clearStop()

Clears linkage to another animation that causes the receiver to stop.

