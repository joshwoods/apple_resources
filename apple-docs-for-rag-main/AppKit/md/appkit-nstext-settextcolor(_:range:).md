

- AppKit
- NSText
-  setTextColor(\_:range:) 

Instance Method

# setTextColor(\_:range:)

Sets the text color of characters within the specified range to the specified color.

macOS

``` source
@MainActor
func setTextColor(
    _ color: NSColor?,
    range: NSRange
)
```

## Discussion

Removes the text color attribute if `color` is `nil`. This method applies only to rich text objects.

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

## See Also

### Setting text color

var textColor: NSColor?

The text color of all characters in the receiver.

