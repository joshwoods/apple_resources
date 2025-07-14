

- AppKit
- NSMenuItem
-  keyEquivalent 

Instance Property

# keyEquivalent

The menu item’s unmodified key equivalent.

macOS

``` source
var keyEquivalent: String { get set }
```

## Discussion

If you want to specify the Backspace key as the key equivalent for a menu item, use a single character string with NSBackspaceCharacter (defined in `NSText.h` as `0x08`) and for the Forward Delete key, use NSDeleteCharacter (defined in `NSText.h` as `0x7F`). Note that these are not the same characters you get from an NSEvent key-down event when pressing those keys.

## See Also

### Related Documentation

var userKeyEquivalent: String

The user-assigned key equivalent for the menu item.

### Managing key equivalents

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The menu item’s keyboard equivalent modifiers.

