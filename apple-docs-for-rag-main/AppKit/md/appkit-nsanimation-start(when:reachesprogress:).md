

- AppKit
- NSAnimation
-  start(when:reachesProgress:) 

Instance Method

# start(when:reachesProgress:)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

macOS

``` source
func start(
    when animation: NSAnimation,
    reachesProgress startProgress: NSAnimation.Progress
)
```

## Parameters 

`animation`  

The other `NSAnimation` object with which the receiver is linked.

`startProgress`  

A `float` value (typed as NSAnimationProgress) that specifies a progress mark of the other animation.

## Discussion

This method links the running of two animations together. You can set only one `NSAnimation` object as a start animation and one as a stop animation at any one time. Setting a new start animation removes any animation previously set.

## See Also

### Related Documentation

func start()

Starts the animation represented by the receiver.

### Linking Animations Together

func stop(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

func clearStart()

Clears linkage to another animation that causes the receiver to start.

func clearStop()

Clears linkage to another animation that causes the receiver to stop.

