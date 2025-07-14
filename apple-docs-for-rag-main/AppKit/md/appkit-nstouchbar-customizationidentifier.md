

- AppKit
- NSTouchBar
-  customizationIdentifier 

Instance Property

# customizationIdentifier

A globally unique string that makes the Touch Bar eligible for user customization.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var customizationIdentifier: NSTouchBar.CustomizationIdentifier? { get set }
```

## Discussion

To make an NSTouchBar object eligible for user customization, assign it a globally unique customizationIdentifier identifier. For the identifier string, use reverse-DNS style, such as “`com.company-name.app-name.alphanumeric-ID`”.

The system archives this property.

## See Also

### Configuring user customization

var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier]

A list of identifiers for items to show in the Touch Bar’s customization UI.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

typealias CustomizationIdentifier

The default type for a Touch Bar customization identifier.

class var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

