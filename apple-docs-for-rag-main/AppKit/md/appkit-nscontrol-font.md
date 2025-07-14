

- AppKit
- NSControl
-  font 

Instance Property

# font

The font used to draw text in the receiver’s cell.

macOS

``` source
@NSCopying @MainActor
var font: NSFont? { get set }
```

## Discussion

If the cell is being edited, setting this property causes the text in the cell to be redrawn in the new font, and the cell’s editor (the `NSText` object used globally for editing) is updated with the new font object.

## See Also

### Formatting Text

var alignment: NSTextAlignment

The alignment mode of the text in the receiver’s cell.

var lineBreakMode: NSLineBreakMode

The line break mode to use for text in the control’s cell.

var usesSingleLineMode: Bool

A Boolean value that indicates whether the text in the control’s cell uses single line mode.

var formatter: Formatter?

The receiver’s formatter.

var baseWritingDirection: NSWritingDirection

The initial writing direction used to determine the actual writing direction for text.

