

- UIKit
- UIBarButtonItemGroup
-  init(barButtonItems:representativeItem:) 

Initializer

# init(barButtonItems:representativeItem:)

Creates a fixed group with the specified items.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(
    barButtonItems: [UIBarButtonItem],
    representativeItem: UIBarButtonItem?
)
```

## Parameters 

`barButtonItems`  

The bar button items to display on the bar. Typically, the items in a group are related to each other in some way, although that need not be the case. You must not specify an empty array.

`representativeItem`  

A bar button item to display when there isn’t enough room to display the items in `barButtonItems`. The object you specify must be distinct from the objects in the `barButtonItems` parameter. It’s a programmer error to specify an object that’s also in the array passed to the `barButtonItems` parameter. You may specify `nil` for this parameter.

## Return Value

An initialized bar button item group.

## Discussion

When you use this initializer to create a group for a navigation bar, it produces the same result as fixedGroup(representativeItem:items:) (Swift) or fixedGroupWithRepresentativeItem:items: (Objective-C).

When you use this initializer to create a group for the shortcuts bar, use the resulting group object to configure the leadingBarButtonGroups or trailingBarButtonGroups property of a UITextInputAssistantItem object.

## See Also

### Creating a group

class func fixedGroup(representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a fixed group that a person can’t move or remove from the navigation bar during layout customization.

class func movableGroup(customizationIdentifier: String, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a movable group that a person can move but can’t remove from the navigation bar during layout customization.

class func optionalGroup(customizationIdentifier: String, isInDefaultCustomization: Bool, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

init?(coder: NSCoder)

Creates a bar button item group from data in an unarchiver.

