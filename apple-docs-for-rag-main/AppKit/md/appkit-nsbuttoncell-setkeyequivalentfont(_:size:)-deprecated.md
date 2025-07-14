

- AppKit
- NSButtonCell
-  setKeyEquivalentFont(\_:size:) Deprecated

Instance Method

# setKeyEquivalentFont(\_:size:)

Sets by name and size of the font used to draw the key equivalent.

macOS 10.0–10.15Deprecated

``` source
@MainActor
func setKeyEquivalentFont(
    _ fontName: String,
    size fontSize: CGFloat
)
```

Deprecated

The keyEquivalentFont property is no longer used. Setting it has no effect.

## Parameters 

`fontName`  

The name of the font to use to draw the key equivalent.

`fontSize`  

The font size to use to draw the key equivalent.

## Discussion

This method redisplays the button if necessary. It does nothing if the button doesn’t have a key equivalent associated with it. The default font is the same as that used to draw the title.

## See Also

### Related Documentation

var font: NSFont?

The font that the cell uses to display text.

### Managing the Key Equivalent

var keyEquivalent: String

The button’s key-equivalent character.

var keyEquivalentFont: NSFont?

The font used to draw the button’s key equivalent.

Deprecated

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The mask that identifies the modifier keys for the button’s key equivalent.

