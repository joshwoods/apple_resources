

- UIKit
- UIFieldBehavior
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Associates the field behavior with the specified dynamic item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func addItem(_ item: any UIDynamicItem)
```

## Parameters 

`item`  

The dynamic item whose behavior you want to modify.

## Discussion

Use this method to apply a field to a dynamic item in your interface. This method adds the specified dynamic item to the field behavior’s list of dynamic items.

## See Also

### Managing the associated dynamic items

func removeItem(any UIDynamicItem)

Removes the field behavior from the specified dynamic item.

var items: [any UIDynamicItem]

The dynamic items associated with the current field behavior.

