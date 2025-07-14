

- UIKit
- UIFieldBehavior
-  removeItem(\_:) 

Instance Method

# removeItem(\_:)

Removes the field behavior from the specified dynamic item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func removeItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item whose behavior you want to modify.

## Discussion

Use this method to remove a field from a dynamic item in your interface. This method removes the specified dynamic item from the field behavior’s list of dynamic item.

## See Also

### Managing the associated dynamic items

func addItem(any UIDynamicItem)

Associates the field behavior with the specified dynamic item.

var items: [any UIDynamicItem]

The dynamic items associated with the current field behavior.

