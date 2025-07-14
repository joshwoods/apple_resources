

- UIKit
- UIViewAnimating
-  state 

Instance Property

# state

The current state of the animation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var state: UIViewAnimatingState { get }
```

**Required**

## Discussion

This property reflects the current state of the animation. An animator object starts in the UIViewAnimatingState.inactive state. Calling the startAnimation() or pauseAnimation() method changes the state to UIViewAnimatingState.active. Changing the fractionComplete property also moves the animator to the active state. The animator remains in the active state until its animations finish, at which point it moves back to the inactive state.

Calling the stopAnimation(_:) method changes the state of the animator to UIViewAnimatingState.stopped. When in this state, the animations are stopped and cannot be restarted until you call the finishAnimation(at:) method, which returns the animator to the inactive state.

## See Also

### Getting the animator’s state

var fractionComplete: CGFloat

The completion percentage of the animation.

**Required**

var isReversed: Bool

A Boolean value indicating whether the animation is running in the reverse direction.

**Required**

var isRunning: Bool

A Boolean value indicating whether the animation is currently running.

**Required**

