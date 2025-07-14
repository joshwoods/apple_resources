

- UIKit
- UIDynamicAnimator
-  updateItem(usingCurrentState:) 

Instance Method

# updateItem(usingCurrentState:)

Asks a dynamic animator to read the current state of a dynamic item, replacing the animator’s internal representation of the item’s state.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func updateItem(usingCurrentState item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item whose state was changed by your app.

## Discussion

A dynamic animator automatically reads the initial state (position and rotation) of each dynamic item you add to it, and then takes responsibility for updating the item’s state. If you actively change the state of a dynamic item *after* you’ve added it to a dynamic animator, call this method to ask the animator to read and incorporate the new state.

## See Also

### Accessing a dynamic animator’s state

var elapsedTime: TimeInterval

Returns the time interval since the dynamic animator started running.

var isRunning: Bool

Returns true if the dynamic animator is running.

var behaviors: [UIDynamicBehavior]

The dynamic behaviors managed by a dynamic animator.

var referenceView: UIView?

The view that a dynamic animator was initialized with.

