

- UIKit
- UIPushBehavior
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Adds a dynamic item to the behavior’s dynamic item array.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item to add to the item array.

## Discussion

All the dynamic items added to a push behavior are subject to the same force vector.

## See Also

### Initializing and managing a push behavior

var active: Bool

The state of the push behavior’s force: either active or inactive.

init(items: [any UIDynamicItem], mode: UIPushBehavior.Mode)

Initializes a push behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the push behavior.

