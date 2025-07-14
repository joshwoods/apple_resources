

- UIKit
- UIBarButtonItem
-  creatingMovableGroup(customizationIdentifier:) 

Instance Method

# creatingMovableGroup(customizationIdentifier:)

Places the item in a movable group that a person can move but can’t remove from the navigation bar during layout customization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func creatingMovableGroup(customizationIdentifier: String) -> UIBarButtonItemGroup
```

## Parameters 

`customizationIdentifier`  

A unique string to identify the group for navigation bar layout customization.

## Return Value

A UIBarButtonItemGroup that contains only this bar button item.

## Discussion

A bar button item can only belong to one UIBarButtonItemGroup. If you add a bar button item to a new group, the system removes it from its previous group.

## See Also

### Creating groups

func creatingOptionalGroup(customizationIdentifier: String, isInDefaultCustomization: Bool) -> UIBarButtonItemGroup

Places the item in an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

func creatingFixedGroup() -> UIBarButtonItemGroup

Places the item in a fixed group that a person can’t move or remove from the navigation bar during layout customization.

