

- UIKit
- UIDynamicItemBehavior
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Adds a dynamic item to the dynamic item behavior’s item array.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item to add to the item array.

## Discussion

You can add a dynamic item to one or more dynamic item behaviors. For example, you could add a dynamic item to one dynamic item behavior to configure the item’s elasticity and to a second dynamic item behavior to configure its density. This is especially useful when you are defining custom, combined behaviors for your dynamic items.

## See Also

### Initializing and managing a dynamic item behavior

init(items: [any UIDynamicItem])

Initializes a dynamic item behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the dynamic item behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the dynamic item behavior.

