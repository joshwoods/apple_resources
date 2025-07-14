

- UIKit
- UIDynamicAnimator
-  isRunning 

Instance Property

# isRunning

Returns true if the dynamic animator is running.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var isRunning: Bool { get }
```

## Discussion

The views associated with an animator’s behaviors can change position or change transform only when the animator is running. For optimization purposes, iOS can pause and then restart an animator. Use this method if you need to check whether or not your views are currently subject to changes in position or transform.

## See Also

### Accessing a dynamic animator’s state

var elapsedTime: TimeInterval

Returns the time interval since the dynamic animator started running.

var behaviors: [UIDynamicBehavior]

The dynamic behaviors managed by a dynamic animator.

var referenceView: UIView?

The view that a dynamic animator was initialized with.

func updateItem(usingCurrentState: any UIDynamicItem)

Asks a dynamic animator to read the current state of a dynamic item, replacing the animator’s internal representation of the item’s state.

