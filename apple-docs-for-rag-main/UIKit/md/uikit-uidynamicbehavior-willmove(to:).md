

- UIKit
- UIDynamicBehavior
-  willMove(to:) 

Instance Method

# willMove(to:)

Called when the dynamic behavior is added to, or removed from, a dynamic animator.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func willMove(to dynamicAnimator: UIDynamicAnimator?)
```

## Parameters 

`dynamicAnimator`  

The dynamic animator that the behavior is being added to, or `nil` if being removed from an animator.

## Discussion

Use this method as the override point for responding to changes in the UIKit Dynamics behavior tree that involve the dynamic behavior.

## See Also

### Responding to changes in the behavior tree

var dynamicAnimator: UIDynamicAnimator?

The dynamic animator that the dynamic behavior is associated with.

