

- UIKit
- UIViewAnimating
-  isReversed 

Instance Property

# isReversed

A Boolean value indicating whether the animation is running in the reverse direction.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isReversed: Bool { get set }
```

**Required**

## Discussion

When the value of this property is true, animations run in the reverse direction—that is, view properties animate back to their original values. When the value is false, view properties animate to their intended final values.

When implementing this property, changes should cause the animation to reverse direction. If you allow changes while the animation is running, it is best to pause the animation briefly and then start it again in the opposite direction. Once the animation transitions to the UIViewAnimatingState.stopped state, you can ignore changes to this property.

## See Also

### Getting the animator’s state

var fractionComplete: CGFloat

The completion percentage of the animation.

**Required**

var state: UIViewAnimatingState

The current state of the animation.

**Required**

var isRunning: Bool

A Boolean value indicating whether the animation is currently running.

**Required**

