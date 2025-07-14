

- UIKit
- UIDynamicItemBehavior
-  items 

Instance Property

# items

Returns the set of dynamic items you’ve added to the dynamic item behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [any UIDynamicItem] { get }
```

## Discussion

## See Also

### Initializing and managing a dynamic item behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the dynamic item behavior’s item array.

init(items: [any UIDynamicItem])

Initializes a dynamic item behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the dynamic item behavior.

