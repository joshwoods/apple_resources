

- UIKit
- UIViewAnimating
-  pauseAnimation() 

Instance Method

# pauseAnimation()

Pauses a running animation at its current position.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func pauseAnimation()
```

**Required**

## Discussion

This method pauses running animations at their current values. Calling this method on an inactive animator moves its state to UIViewAnimatingState.active and puts its animations in a paused state right away. To resume the animations, call the startAnimation() method. If the animation is already paused, this method should do nothing. It is a programmer error to call this method while the state of the animator is set to UIViewAnimatingState.stopped.

## See Also

### Starting and stopping the animations

func startAnimation()

Starts the animation from its current position.

**Required**

func startAnimation(afterDelay: TimeInterval)

Starts the animation after the specified delay.

**Required**

func stopAnimation(Bool)

Stops the animations at their current positions.

**Required**

func finishAnimation(at: UIViewAnimatingPosition)

Finishes the animations and returns the animator to the inactive state.

**Required**

