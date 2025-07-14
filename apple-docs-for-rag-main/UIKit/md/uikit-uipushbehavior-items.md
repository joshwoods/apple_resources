

- UIKit
- UIPushBehavior
-  items 

Instance Property

# items

Returns the set of dynamic items you’ve added to the push behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [any UIDynamicItem] { get }
```

## See Also

### Initializing and managing a push behavior

var active: Bool

The state of the push behavior’s force: either active or inactive.

func addItem(any UIDynamicItem)

Adds a dynamic item to the behavior’s dynamic item array.

init(items: [any UIDynamicItem], mode: UIPushBehavior.Mode)

Initializes a push behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the behavior.

