

- AppKit
- NSTouchBar
-  escapeKeyReplacementItemIdentifier 

Instance Property

# escapeKeyReplacementItemIdentifier

The identifier of an item that replaces the system-provided button in the Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var escapeKeyReplacementItemIdentifier: NSTouchBarItem.Identifier? { get set }
```

## Discussion

To replace the system-provided button, set escapeKeyReplacementItemIdentifier to the identifier of an NSTouchBarItem instance. You must also include the item instance in the Touch Bar’s templateItems array, or return the item when the Touch Bar calls the touchBar(_:makeItemForIdentifier:) delegate method.

Devices that include the Touch Bar (second generation) have a dedicated Escape key located to the left of the Touch Bar. By default, the Touch Bar hides the system-provided button and its replacement on these devices. However, if you set the replacement item’s visibilityPriority to high, the Touch Bar shows the item and reduces the visible space of the app region.

## See Also

### Providing bar items

var delegate: (any NSTouchBarDelegate)?

The delegate that provides items to the Touch Bar.

var templateItems: Set&lt;NSTouchBarItem>

The primary source of items that the Touch Bar uses to fill its private items array, unless you provide items using a delegate.

var defaultItemIdentifiers: [NSTouchBarItem.Identifier]

A required list of identifiers for items that you want to appear in the Touch Bar after instantiating it.

var principalItemIdentifier: NSTouchBarItem.Identifier?

The identifier of an item you want the system to center in the Touch Bar.

