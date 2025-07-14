

- UIKit
- UIBarButtonItem
-  creatingOptionalGroup(customizationIdentifier:isInDefaultCustomization:) 

Instance Method

# creatingOptionalGroup(customizationIdentifier:isInDefaultCustomization:)

Places the item in an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func creatingOptionalGroup(
    customizationIdentifier: String,
    isInDefaultCustomization: Bool = true
) -> UIBarButtonItemGroup
```

## Parameters 

`customizationIdentifier`  

A unique string to identify the group for navigation bar layout customization.

`isInDefaultCustomization`  

A Boolean that determines whether to place the group in the navigation bar by default. Specify false if you want the group to appear in the navigation bar customization popover by default.

## Return Value

A UIBarButtonItemGroup that contains only this bar button item.

## Discussion

A bar button item can only belong to one UIBarButtonItemGroup. If you add a bar button item to a new group, the system removes it from its previous group.

## See Also

### Creating groups

func creatingFixedGroup() -> UIBarButtonItemGroup

Places the item in a fixed group that a person can’t move or remove from the navigation bar during layout customization.

func creatingMovableGroup(customizationIdentifier: String) -> UIBarButtonItemGroup

Places the item in a movable group that a person can move but can’t remove from the navigation bar during layout customization.

