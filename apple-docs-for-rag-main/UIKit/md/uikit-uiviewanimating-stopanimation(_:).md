

- UIKit
- UIViewAnimating
-  stopAnimation(\_:) 

Instance Method

# stopAnimation(\_:)

Stops the animations at their current positions.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func stopAnimation(_ withoutFinishing: Bool)
```

**Required**

## Parameters 

`withoutFinishing`  

A Boolean indicating whether any final actions should be performed. Specify true to clear any animations and move the animator directly to the UIViewAnimatingState.inactive state without performing any final actions. Specify false to put the animator into the UIViewAnimatingState.stopped state.

## Discussion

Call this method when you want to end the animations at their current position. This method removes all of the associated animations from the execution stack and sets the values of any animatable properties to their current values. This method also updates the state of the animator object based on the value of the `withoutFinishing` parameter.

If you specify false for the `withoutFinishing` parameter, you can subsequently call the finishAnimation(at:) method to perform the animator’s final actions. For example, a UIViewPropertyAnimator object executes its completion blocks when you call this method. You do not have to call the finishAnimation(at:) method right away, or at all, and you can perform other animations before calling that method.

## See Also

### Starting and stopping the animations

func startAnimation()

Starts the animation from its current position.

**Required**

func startAnimation(afterDelay: TimeInterval)

Starts the animation after the specified delay.

**Required**

func pauseAnimation()

Pauses a running animation at its current position.

**Required**

func finishAnimation(at: UIViewAnimatingPosition)

Finishes the animations and returns the animator to the inactive state.

**Required**

