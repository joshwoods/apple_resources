

- AppKit
- NSTouchBar
-  customizationAllowedItemIdentifiers 

Instance Property

# customizationAllowedItemIdentifiers

A list of identifiers for items to show in the Touch Bar’s customization UI.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier] { get set }
```

## Discussion

The customization UI shows these items in additional to the items in defaultItemIdentifiers.

The items you include in customizationAllowedItemIdentifiers appear individually in the customization UI, arranged in the same order as you specify in the array. As long as there’s available geometric space, a user can drag in to the associated bar any of the items in this list.

Always configure this property for a customizable bar.

The system archives this property.

## See Also

### Related Documentation

var defaultItemIdentifiers: [NSTouchBarItem.Identifier]

A required list of identifiers for items that you want to appear in the Touch Bar after instantiating it.

var itemIdentifiers: [NSTouchBarItem.Identifier]

The list of identifiers for the current items in the Touch Bar.

### Configuring user customization

var customizationIdentifier: NSTouchBar.CustomizationIdentifier?

A globally unique string that makes the Touch Bar eligible for user customization.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

typealias CustomizationIdentifier

The default type for a Touch Bar customization identifier.

class var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

