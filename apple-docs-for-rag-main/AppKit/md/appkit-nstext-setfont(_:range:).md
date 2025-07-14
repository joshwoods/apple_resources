

- AppKit
- NSText
-  setFont(\_:range:) 

Instance Method

# setFont(\_:range:)

Sets the font of characters within `aRange` to `aFont`.

macOS

``` source
@MainActor
func setFont(
    _ font: NSFont,
    range: NSRange
)
```

## Discussion

This method applies only to a rich text object.

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

## See Also

### Changing the font

func changeFont(Any?)

This action method changes the font of the selection for a rich text object, or of all text for a plain text object.

var font: NSFont?

The font of all the receiver’s text.

