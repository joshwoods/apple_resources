

- AppKit
- NSTouchBar
-  delegate 

Instance Property

# delegate

The delegate that provides items to the Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
weak var delegate: (any NSTouchBarDelegate)? { get set }
```

## Discussion

Employ a bar delegate, according to the needs of your app, to dynamically create items (NSTouchBarItem instances). For more information, see Item objects.

This property is conditionally archived, as described in the encodeConditionalObject(_:forKey:) method.

## See Also

### Providing bar items

var templateItems: Set&lt;NSTouchBarItem>

The primary source of items that the Touch Bar uses to fill its private items array, unless you provide items using a delegate.

var defaultItemIdentifiers: [NSTouchBarItem.Identifier]

A required list of identifiers for items that you want to appear in the Touch Bar after instantiating it.

var principalItemIdentifier: NSTouchBarItem.Identifier?

The identifier of an item you want the system to center in the Touch Bar.

var escapeKeyReplacementItemIdentifier: NSTouchBarItem.Identifier?

The identifier of an item that replaces the system-provided button in the Touch Bar.

