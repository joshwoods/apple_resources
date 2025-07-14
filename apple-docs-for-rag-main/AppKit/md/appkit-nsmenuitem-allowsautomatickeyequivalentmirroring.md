

- AppKit
- NSMenuItem
-  allowsAutomaticKeyEquivalentMirroring 

Instance Property

# allowsAutomaticKeyEquivalentMirroring

A Boolean value that determines whether the system automatically swaps input strings for some keyboard shortcuts when the interface direction changes.

macOS 12.0+

``` source
var allowsAutomaticKeyEquivalentMirroring: Bool { get set }
```

## Discussion

When a menu item represents a direction-related action, it’s common to specify an input string that conveys that direction. For example, Finder uses Command-\[ to go back to the previous page, and Command-\] to go forward to the next page. Because directions are different in left-to-right and right-to-left interfaces, this property lets the system swap some input strings to match the current language direction.

When the value of this property is true, macOS 12 and later automatically swaps input strings that contain brackets `[]`, braces `{}`, parenthesis `()`, angle brackets `<>`, or arrow keys when the interface directionality changes. This behavior eliminates the need for you to create different menu items for left-to-right and right-to-left interfaces. Set this property to false if you already change this item’s shortcut to support both left-to-right and right-to-left interfaces. You might also set it to false to keep the same shortcut regardless of the interface’s directionality.

The default value of this property is true. However, if you set the allowsAutomaticLocalization property to false, the system disables this feature regardless of the property’s value.

## See Also

### Managing user key equivalents

class var usesUserKeyEquivalents: Bool

Returns a Boolean value that indicates whether menu items conform to user preferences for key equivalents.

var userKeyEquivalent: String

The user-assigned key equivalent for the menu item.

var allowsAutomaticKeyEquivalentLocalization: Bool

A Boolean value that determines whether the system automatically remaps the keyboard shortcut to support localized keyboards.

var allowsKeyEquivalentWhenHidden: Bool

