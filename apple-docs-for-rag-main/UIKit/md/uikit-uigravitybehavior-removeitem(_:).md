

- UIKit
- UIGravityBehavior
-  removeItem(\_:) 

Instance Method

# removeItem(\_:)

Removes the specified dynamic item from the gravity behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item that you want to remove. If the specified item is not associated with the behavior, this method does nothing.

## Discussion

If the gravity behavior has an associated dynamic animator, this method notifies the dynamic animator of the removal of the item so that it can stop any associated animations.

## See Also

### Managing a gravity behavior’s items

var items: [any UIDynamicItem]

The set of dynamic items associated with the gravity behavior.

func addItem(any UIDynamicItem)

Associates the specified dynamic item with the gravity behavior.

