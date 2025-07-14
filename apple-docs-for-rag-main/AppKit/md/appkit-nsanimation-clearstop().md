

- AppKit
- NSAnimation
-  clearStop() 

Instance Method

# clearStop()

Clears linkage to another animation that causes the receiver to stop.

macOS

``` source
func clearStop()
```

## Discussion

The linkage to the other animation is made with stop(when:reachesProgress:).

## See Also

### Related Documentation

func stop()

Stops the animation represented by the receiver.

### Linking Animations Together

func start(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

func stop(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

func clearStart()

Clears linkage to another animation that causes the receiver to start.

