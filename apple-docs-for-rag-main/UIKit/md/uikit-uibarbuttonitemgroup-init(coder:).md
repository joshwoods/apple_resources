

- UIKit
- UIBarButtonItemGroup
-  init(coder:) 

Initializer

# init(coder:)

Creates a bar button item group from data in an unarchiver.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a group

class func fixedGroup(representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a fixed group that a person can’t move or remove from the navigation bar during layout customization.

class func movableGroup(customizationIdentifier: String, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a movable group that a person can move but can’t remove from the navigation bar during layout customization.

class func optionalGroup(customizationIdentifier: String, isInDefaultCustomization: Bool, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

init(barButtonItems: [UIBarButtonItem], representativeItem: UIBarButtonItem?)

Creates a fixed group with the specified items.

