

- UIKit
- UIDynamicItemBehavior
-  init(items:) 

Initializer

# init(items:)

Initializes a dynamic item behavior with an array of dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(items: [any UIDynamicItem])
```

## Parameters 

`items`  

The dynamic items that you want to be subject to the dynamic item behavior.

## Return Value

The initialized dynamic item behavior, or `nil` if there was a problem initializing the object.

## See Also

### Initializing and managing a dynamic item behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the dynamic item behavior’s item array.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the dynamic item behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the dynamic item behavior.

