

- AppKit
- NSMenuItem
-  usesUserKeyEquivalents 

Type Property

# usesUserKeyEquivalents

Returns a Boolean value that indicates whether menu items conform to user preferences for key equivalents.

macOS

``` source
class var usesUserKeyEquivalents: Bool { get set }
```

## Return Value

true if menu items conform to user preferences for key equivalents; otherwise, false.

## See Also

### Managing user key equivalents

var userKeyEquivalent: String

The user-assigned key equivalent for the menu item.

var allowsAutomaticKeyEquivalentLocalization: Bool

A Boolean value that determines whether the system automatically remaps the keyboard shortcut to support localized keyboards.

var allowsAutomaticKeyEquivalentMirroring: Bool

A Boolean value that determines whether the system automatically swaps input strings for some keyboard shortcuts when the interface direction changes.

var allowsKeyEquivalentWhenHidden: Bool

