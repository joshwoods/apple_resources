

- UIKit
- UIDynamicAnimator
-  behaviors 

Instance Property

# behaviors

The dynamic behaviors managed by a dynamic animator.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var behaviors: [UIDynamicBehavior] { get }
```

## See Also

### Accessing a dynamic animator’s state

var elapsedTime: TimeInterval

Returns the time interval since the dynamic animator started running.

var isRunning: Bool

Returns true if the dynamic animator is running.

var referenceView: UIView?

The view that a dynamic animator was initialized with.

func updateItem(usingCurrentState: any UIDynamicItem)

Asks a dynamic animator to read the current state of a dynamic item, replacing the animator’s internal representation of the item’s state.

