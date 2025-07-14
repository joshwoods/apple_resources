

- AppKit
- NSTouchBar
-  isAutomaticCustomizeTouchBarMenuItemEnabled 

Type Property

# isAutomaticCustomizeTouchBarMenuItemEnabled

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
class var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, AppKit adds a standard item to the app’s View menu that users can select to customize the Touch Bar contents, but only if a Touch Bar is present. If the View menu is unavailable, AppKit adds the item to either the Windows or App menu.

If you prefer to provide a customize menu item, set isAutomaticCustomizeTouchBarMenuItemEnabled to false, and create the menu item with an action of toggleTouchBarCustomizationPalette(_:).

The default value of this property is false.

## See Also

### Configuring user customization

var customizationIdentifier: NSTouchBar.CustomizationIdentifier?

A globally unique string that makes the Touch Bar eligible for user customization.

var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier]

A list of identifiers for items to show in the Touch Bar’s customization UI.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

typealias CustomizationIdentifier

The default type for a Touch Bar customization identifier.

