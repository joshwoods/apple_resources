

- AppKit
- NSButtonCell
-  keyEquivalentFont Deprecated

Instance Property

# keyEquivalentFont

The font used to draw the button’s key equivalent.

macOS 10.0–10.15Deprecated

``` source
@MainActor
var keyEquivalentFont: NSFont? { get set }
```

Deprecated

The keyEquivalentFont property is no longer used. It always returns the NSButtonCell's font, and setting it has no effect.

## Discussion

The value of this property is the font object that describes the font used to draw the button’s key equivalent. If the property value is `nil`, the button doesn’t have a key equivalent. Setting this property redraws the button if necessary. Setting this property on a button that has no key equivalent does nothing.

Note that the default font is the same as the font used to draw the title.

## See Also

### Related Documentation

var font: NSFont?

The font that the cell uses to display text.

### Managing the Key Equivalent

var keyEquivalent: String

The button’s key-equivalent character.

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The mask that identifies the modifier keys for the button’s key equivalent.

func setKeyEquivalentFont(String, size: CGFloat)

Sets by name and size of the font used to draw the key equivalent.

Deprecated

