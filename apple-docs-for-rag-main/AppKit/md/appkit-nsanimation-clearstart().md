

- AppKit
- NSAnimation
-  clearStart() 

Instance Method

# clearStart()

Clears linkage to another animation that causes the receiver to start.

macOS

``` source
func clearStart()
```

## Discussion

The linkage to the other animation is made with start(when:reachesProgress:).

## See Also

### Related Documentation

func start()

Starts the animation represented by the receiver.

### Linking Animations Together

func start(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

func stop(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

func clearStop()

Clears linkage to another animation that causes the receiver to stop.

