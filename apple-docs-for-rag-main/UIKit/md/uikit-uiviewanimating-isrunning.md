

- UIKit
- UIViewAnimating
-  isRunning 

Instance Property

# isRunning

A Boolean value indicating whether the animation is currently running.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isRunning: Bool { get }
```

**Required**

## Discussion

This property reflects whether the animation is running either in the forward or reverse direction. The value of this property is true only after a call to the startAnimation() method. The value is false when the animator is paused or stopped.

## See Also

### Getting the animator’s state

var fractionComplete: CGFloat

The completion percentage of the animation.

**Required**

var isReversed: Bool

A Boolean value indicating whether the animation is running in the reverse direction.

**Required**

var state: UIViewAnimatingState

The current state of the animation.

**Required**

