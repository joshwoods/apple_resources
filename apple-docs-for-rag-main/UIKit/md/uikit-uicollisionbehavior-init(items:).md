

- UIKit
- UICollisionBehavior
-  init(items:) 

Initializer

# init(items:)

Initializes a collision behavior with an array of dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(items: [any UIDynamicItem])
```

## Parameters 

`items`  

The dynamic items that you want to participate in the collision behavior.

## Return Value

The initialized collision behavior, or `nil` if there was a problem initializing the object.

## See Also

### Initializing and managing a collision behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the collision behavior’s item array.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the collision behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the collision behavior.

