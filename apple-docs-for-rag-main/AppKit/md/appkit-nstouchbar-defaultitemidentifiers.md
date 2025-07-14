

- AppKit
- NSTouchBar
-  defaultItemIdentifiers 

Instance Property

# defaultItemIdentifiers

A required list of identifiers for items that you want to appear in the Touch Bar after instantiating it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var defaultItemIdentifiers: [NSTouchBarItem.Identifier] { get set }
```

## Discussion

Always specify this property for an NSTouchBar object, even if you elect to make the bar noncustomizable. The system:

- Shows this list’s items by default when the system displays the bar.

- Includes a preconfigured bar, containing these items, in the associated customization UI (when you have assigned the bar a customizationIdentifier property value); the user can drag the default bar into the Touch Bar, should they want to return to the default configuration.

The system archives this property.

## See Also

### Related Documentation

var customizationIdentifier: NSTouchBar.CustomizationIdentifier?

A globally unique string that makes the Touch Bar eligible for user customization.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier]

A list of identifiers for items to show in the Touch Bar’s customization UI.

var itemIdentifiers: [NSTouchBarItem.Identifier]

The list of identifiers for the current items in the Touch Bar.

### Providing bar items

var delegate: (any NSTouchBarDelegate)?

The delegate that provides items to the Touch Bar.

var templateItems: Set&lt;NSTouchBarItem>

The primary source of items that the Touch Bar uses to fill its private items array, unless you provide items using a delegate.

var principalItemIdentifier: NSTouchBarItem.Identifier?

The identifier of an item you want the system to center in the Touch Bar.

var escapeKeyReplacementItemIdentifier: NSTouchBarItem.Identifier?

The identifier of an item that replaces the system-provided button in the Touch Bar.

