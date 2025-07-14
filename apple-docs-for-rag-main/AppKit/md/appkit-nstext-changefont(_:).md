

- AppKit
- NSText
-  changeFont(\_:) 

Instance Method

# changeFont(\_:)

This action method changes the font of the selection for a rich text object, or of all text for a plain text object.

macOS

``` source
@MainActor
func changeFont(_ sender: Any?)
```

## Discussion

If the receiver doesn’t use the Font panel, this method does nothing.

This method changes the font by sending a convert(_:) message to the shared NSFontManager and applying each NSFont returned to the appropriate text. See the NSFontManager class specification for more information on font conversion.

## See Also

### Related Documentation

var usesFontPanel: Bool

A Boolean that controls whether the receiver uses the Font panel and Font menu.

### Changing the font

var font: NSFont?

The font of all the receiver’s text.

func setFont(NSFont, range: NSRange)

Sets the font of characters within `aRange` to `aFont`.

