

- AppKit
- NSTextField
-  lineBreakStrategy 

Instance Property

# lineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

macOS 10.15+

``` source
@MainActor
var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy { get set }
```

## Discussion

The default value for editable text fields is NSLineBreakStrategyNone to match the field editor’s behavior. The default value for selectable, uneditable text fields is standard.

Note

When the text field has an attributed string value, the system ignores the textColor, font, alignment, lineBreakMode, and `lineBreakStrategy` properties. Set the foregroundColor, font, alignment, lineBreakMode, and lineBreakStrategy properties in the attributed string instead.

## See Also

### Configuring Line Wrapping

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that controls whether single-line text fields tighten intercharacter spacing before truncating the text.

var maximumNumberOfLines: Int

The maximum number of lines a wrapping text field displays before clipping or truncating the text.

