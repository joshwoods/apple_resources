

- UIKit
- UICollisionBehavior
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Adds a dynamic item to the collision behavior’s item array.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item to add to the item array.

## Discussion

You can add a dynamic item to one or more collision behaviors. For example, you can use two collision behaviors to specify that item *A* can collide with item *B* and that item *C* can collide with item *D*, but that items *A* and *B* ignore items *C* and *D*.

There is no hard limit to the number of dynamic items you can add to a collision behavior. However, adding a large number of items might result in a performance impact. Be sure to test your behaviors on the device configurations you are targeting.

## See Also

### Initializing and managing a collision behavior

init(items: [any UIDynamicItem])

Initializes a collision behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the collision behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the collision behavior.

