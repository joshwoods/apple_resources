

- AppKit
- NSButtonCell
-  keyEquivalentModifierMask 

Instance Property

# keyEquivalentModifierMask

The mask that identifies the modifier keys for the button’s key equivalent.

macOS

``` source
@MainActor
var keyEquivalentModifierMask: NSEvent.ModifierFlags { get set }
```

## Discussion

The value of this property is a mask that indicates the modifier keys that are applied to the button’s key equivalent. Mask bits are defined in `NSEvent.h`. The only mask bits that are relevant in button key-equivalent modifier masks are `NSControlKeyMask`, `NSAlternateKeyMask`, and `NSCommandKeyMask` bits.

## See Also

### Managing the Key Equivalent

var keyEquivalent: String

The button’s key-equivalent character.

var keyEquivalentFont: NSFont?

The font used to draw the button’s key equivalent.

Deprecated

func setKeyEquivalentFont(String, size: CGFloat)

Sets by name and size of the font used to draw the key equivalent.

Deprecated

