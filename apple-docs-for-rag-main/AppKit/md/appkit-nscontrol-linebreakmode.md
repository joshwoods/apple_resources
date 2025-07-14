

- AppKit
- NSControl
-  lineBreakMode 

Instance Property

# lineBreakMode

The line break mode to use for text in the control’s cell.

macOS 10.10+

``` source
@MainActor
var lineBreakMode: NSLineBreakMode { get set }
```

## Discussion

For a list of possible values, see NSLineBreakMode.

## See Also

### Formatting Text

var alignment: NSTextAlignment

The alignment mode of the text in the receiver’s cell.

var font: NSFont?

The font used to draw text in the receiver’s cell.

var usesSingleLineMode: Bool

A Boolean value that indicates whether the text in the control’s cell uses single line mode.

var formatter: Formatter?

The receiver’s formatter.

var baseWritingDirection: NSWritingDirection

The initial writing direction used to determine the actual writing direction for text.

