

- AppKit
- NSTouchBar
-  NSTouchBar.CustomizationIdentifier 

Type Alias

# NSTouchBar.CustomizationIdentifier

The default type for a Touch Bar customization identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
typealias CustomizationIdentifier = String
```

## See Also

### Configuring user customization

var customizationIdentifier: NSTouchBar.CustomizationIdentifier?

A globally unique string that makes the Touch Bar eligible for user customization.

var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier]

A list of identifiers for items to show in the Touch Bar’s customization UI.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

class var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

