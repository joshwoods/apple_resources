

- UIKit
- UIViewAnimating
-  startAnimation(afterDelay:) 

Instance Method

# startAnimation(afterDelay:)

Starts the animation after the specified delay.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func startAnimation(afterDelay delay: TimeInterval)
```

**Required**

## Parameters 

`delay`  

The amount of time (in seconds) to wait before starting the animation.

## Discussion

Call this method to start the animations or to resume a set of paused animations after the specified time delay. This method sets the state of the animator to UIViewAnimatingState.active, if it is not already there. It is a programmer error to call this method while the state of the animator is set to UIViewAnimatingState.stopped.

When implementing a custom animator, use this method to transition your animator to the active state and to run the animations after the specified delay. Run your animations from the progress point in the fractionComplete property. Update the state and isRunning properties, as well as any other relevant properties of your custom animator object.

## See Also

### Starting and stopping the animations

func startAnimation()

Starts the animation from its current position.

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

