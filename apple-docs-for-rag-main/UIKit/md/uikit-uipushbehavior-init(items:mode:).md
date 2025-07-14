

- UIKit
- UIPushBehavior
-  init(items:mode:) 

Initializer

# init(items:mode:)

Initializes a push behavior with an array of dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    items: [any UIDynamicItem],
    mode: UIPushBehavior.Mode
)
```

## Parameters 

`items`  

The dynamic items that you want to be subject to the push behavior.

`mode`  

The mode for the new push behavior; one of the values defined in the UIPushBehavior.Mode enumeration. You must supply a value.

## Return Value

The initialized push behavior, or `nil` if there was a problem initializing the object.

## See Also

### Initializing and managing a push behavior

var active: Bool

The state of the push behavior’s force: either active or inactive.

func addItem(any UIDynamicItem)

Adds a dynamic item to the behavior’s dynamic item array.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the push behavior.

