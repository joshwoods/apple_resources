

- UIKit
- UIPushBehavior
-  active 

Instance Property

# active

The state of the push behavior’s force: either active or inactive.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var active: Bool { get set }
```

## Discussion

After you’ve added a push behavior to a dynamic animator, use this property to activate or deactivate the behavior’s force (rather than removing and then re-adding the behavior to the animator).

## See Also

### Initializing and managing a push behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the behavior’s dynamic item array.

init(items: [any UIDynamicItem], mode: UIPushBehavior.Mode)

Initializes a push behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the push behavior.

