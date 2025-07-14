

- AppKit
- NSButton
-  keyEquivalentModifierMask 

Instance Property

# keyEquivalentModifierMask

The mask specifying the modifier keys for the button’s key equivalent.

macOS

``` source
@MainActor
var keyEquivalentModifierMask: NSEvent.ModifierFlags { get set }
```

## Discussion

This property contains the mask specifying the modifier keys that are applied to the button’s key equivalent. Mask bits are defined in Modifier Flags. The only mask bits relevant in button key-equivalent modifier masks are `NSControlKeyMask`, `NSAlternateKeyMask`, and `NSCommandKeyMask`.

## See Also

### Accessing Key Equivalents

var keyEquivalent: String

The key-equivalent character of the button.

