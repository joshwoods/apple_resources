

- UIKit
- UICollisionBehavior
-  items 

Instance Property

# items

Returns the set of dynamic items you’ve added to the collision behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [any UIDynamicItem] { get }
```

## See Also

### Initializing and managing a collision behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the collision behavior’s item array.

init(items: [any UIDynamicItem])

Initializes a collision behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the collision behavior.

