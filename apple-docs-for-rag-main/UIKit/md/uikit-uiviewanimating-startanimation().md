

- UIKit
- UIViewAnimating
-  startAnimation() 

Instance Method

# startAnimation()

Starts the animation from its current position.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func startAnimation()
```

**Required**

## Discussion

Call this method to start the animations or to resume the animation after they were paused. This method sets the state of the animator to UIViewAnimatingState.active, if it isn’t already there. It’s a programmer error to call this method while the state of the animator is set to UIViewAnimatingState.stopped.

When implementing a custom animator, use this method to transition your animator to the active state and to run the animations. Run your animations from the progress point in the fractionComplete property. Update the state and isRunning properties, as well as any other relevant properties of your custom animator object.

## See Also

### Starting and stopping the animations

func startAnimation(afterDelay: TimeInterval)

Starts the animation after the specified delay.

**Required**

func pauseAnimation()

Pauses a running animation at its current position.

**Required**

func stopAnimation(Bool)

Stops the animations at their current positions.

**Required**

func finishAnimation(at: UIViewAnimatingPosition)

Finishes the animations and returns the animator to the inactive state.

**Required**

