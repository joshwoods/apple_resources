

- UIKit
- UIDynamicBehavior
-  action 

Instance Property

# action

The block you want to execute during dynamic animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var action: (() -> Void)? { get set }
```

## Discussion

The dynamic animator calls the action block on every animation step.

## See Also

### Related Documentation

func willMove(to: UIDynamicAnimator?)

Called when the dynamic behavior is added to, or removed from, a dynamic animator.

### Configuring a dynamic behavior

func addChildBehavior(UIDynamicBehavior)

Adds a dynamic behavior, as a child, to a custom dynamic behavior.

var childBehaviors: [UIDynamicBehavior]

Returns the array of dynamic behaviors that are children of a custom dynamic behavior.

func removeChildBehavior(UIDynamicBehavior)

Removes a child dynamic behavior from a custom dynamic behavior.

