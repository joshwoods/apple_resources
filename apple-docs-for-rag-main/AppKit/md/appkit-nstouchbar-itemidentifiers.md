

- AppKit
- NSTouchBar
-  itemIdentifiers 

Instance Property

# itemIdentifiers

The list of identifiers for the current items in the Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var itemIdentifiers: [NSTouchBarItem.Identifier] { get }
```

## Discussion

If the user has not customized the bar, this property’s value is the same as that of the defaultItemIdentifiers property.

The system *does not* archive this property.

## See Also

### Related Documentation

var customizationIdentifier: NSTouchBar.CustomizationIdentifier?

A globally unique string that makes the Touch Bar eligible for user customization.

var customizationRequiredItemIdentifiers: [NSTouchBarItem.Identifier]

An optional list of identifiers for items you want to always appear in the Touch Bar and which the user can’t remove during customization.

var customizationAllowedItemIdentifiers: [NSTouchBarItem.Identifier]

A list of identifiers for items to show in the Touch Bar’s customization UI.

var defaultItemIdentifiers: [NSTouchBarItem.Identifier]

A required list of identifiers for items that you want to appear in the Touch Bar after instantiating it.

### Observing bar status

var isVisible: Bool

A Boolean value that Indicates whether the Touch Bar is eligible for display.

func item(forIdentifier: NSTouchBarItem.Identifier) -> NSTouchBarItem?

Returns the Touch Bar item that corresponds to a given identifier.

