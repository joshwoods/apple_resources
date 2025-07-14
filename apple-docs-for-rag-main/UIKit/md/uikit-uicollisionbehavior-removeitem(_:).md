

- UIKit
- UICollisionBehavior
-  removeItem(\_:) 

Instance Method

# removeItem(\_:)

Removes a specific dynamic item from the collision behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item that you want to remove.

## See Also

### Initializing and managing a collision behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the collision behavior’s item array.

init(items: [any UIDynamicItem])

Initializes a collision behavior with an array of dynamic items.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the collision behavior.

