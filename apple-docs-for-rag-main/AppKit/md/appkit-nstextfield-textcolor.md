

- AppKit
- NSTextField
-  textColor 

Instance Property

# textColor

The color of the text field’s content.

macOS

``` source
@NSCopying @MainActor
var textColor: NSColor? { get set }
```

## Discussion

Note

When the text field has an attributed string value, the system ignores the textColor, font, alignment, lineBreakMode, and `lineBreakStrategy` properties. Set the foregroundColor, font, alignment, lineBreakMode, and lineBreakStrategy properties in the attributed string instead.

## See Also

### Related Documentation

var backgroundColor: NSColor?

The color of the background the text field’s cell draws behind the text.

var textColor: NSColor?

The color to use to draw the cell’s text.

