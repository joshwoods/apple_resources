

- UIKit
- UIDynamicAnimator
-  referenceView 

Instance Property

# referenceView

The view that a dynamic animator was initialized with.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var referenceView: UIView? { get }
```

## Discussion

This property has a value only for a dynamic animator initialized using the init(referenceView:) method.

## See Also

### Accessing a dynamic animator’s state

var elapsedTime: TimeInterval

Returns the time interval since the dynamic animator started running.

var isRunning: Bool

Returns true if the dynamic animator is running.

var behaviors: [UIDynamicBehavior]

The dynamic behaviors managed by a dynamic animator.

func updateItem(usingCurrentState: any UIDynamicItem)

Asks a dynamic animator to read the current state of a dynamic item, replacing the animator’s internal representation of the item’s state.

