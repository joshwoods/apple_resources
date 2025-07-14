

- AppKit
- NSMenuItem
-  userKeyEquivalent 

Instance Property

# userKeyEquivalent

The user-assigned key equivalent for the menu item.

macOS

``` source
var userKeyEquivalent: String { get }
```

## See Also

### Related Documentation

var keyEquivalent: String

The menu item’s unmodified key equivalent.

### Managing user key equivalents

class var usesUserKeyEquivalents: Bool

Returns a Boolean value that indicates whether menu items conform to user preferences for key equivalents.

var allowsAutomaticKeyEquivalentLocalization: Bool

A Boolean value that determines whether the system automatically remaps the keyboard shortcut to support localized keyboards.

var allowsAutomaticKeyEquivalentMirroring: Bool

A Boolean value that determines whether the system automatically swaps input strings for some keyboard shortcuts when the interface direction changes.

var allowsKeyEquivalentWhenHidden: Bool

