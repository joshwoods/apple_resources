

- UIKit
- UIGravityBehavior
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Associates the specified dynamic item with the gravity behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item to add to the item array. If the specified item is already associated with the gravity behavior, this method does nothing.

## Discussion

Use this method to add new dynamic items to the gravity behavior after initialization. All the dynamic items added to a gravity behavior are subject to the same gravity vector.

If the gravity behavior has an associated dynamic animator, this method notifies the dynamic animator of the presence of the new item so that it can initiate any needed animations.

## See Also

### Managing a gravity behavior’s items

var items: [any UIDynamicItem]

The set of dynamic items associated with the gravity behavior.

func removeItem(any UIDynamicItem)

Removes the specified dynamic item from the gravity behavior.

