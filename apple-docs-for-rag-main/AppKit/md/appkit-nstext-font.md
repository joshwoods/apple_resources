

- AppKit
- NSText
-  font 

Instance Property

# font

The font of all the receiver’s text.

macOS

``` source
@MainActor
var font: NSFont? { get set }
```

## Discussion

When the specified font doesn’t include a character, the text system uses an alternate font that contains the character. The substituted font may not have compatible metrics.

## See Also

### Changing the font

func changeFont(Any?)

This action method changes the font of the selection for a rich text object, or of all text for a plain text object.

func setFont(NSFont, range: NSRange)

Sets the font of characters within `aRange` to `aFont`.

