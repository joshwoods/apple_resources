

- UIKit
- UIDynamicBehavior
-  dynamicAnimator 

Instance Property

# dynamicAnimator

The dynamic animator that the dynamic behavior is associated with.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var dynamicAnimator: UIDynamicAnimator? { get }
```

## Discussion

If the dynamic behavior is not associated with a dynamic animator, the value of this property is `nil`.

## See Also

### Responding to changes in the behavior tree

func willMove(to: UIDynamicAnimator?)

Called when the dynamic behavior is added to, or removed from, a dynamic animator.

