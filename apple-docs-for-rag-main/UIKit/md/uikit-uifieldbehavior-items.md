

- UIKit
- UIFieldBehavior
-  items 

Instance Property

# items

The dynamic items associated with the current field behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var items: [any UIDynamicItem] { get }
```

## Discussion

When it is enabled, the current field applies its behavior to all of the items in the array.

## See Also

### Managing the associated dynamic items

func addItem(any UIDynamicItem)

Associates the field behavior with the specified dynamic item.

func removeItem(any UIDynamicItem)

Removes the field behavior from the specified dynamic item.

