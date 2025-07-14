

- AppKit
- NSTextField
-  allowsDefaultTighteningForTruncation 

Instance Property

# allowsDefaultTighteningForTruncation

A Boolean value that controls whether single-line text fields tighten intercharacter spacing before truncating the text.

macOS 10.11+

``` source
@MainActor
var allowsDefaultTighteningForTruncation: Bool { get set }
```

## Discussion

The text field ignores this property when its value is an attributed string.

## See Also

### Configuring Line Wrapping

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

var maximumNumberOfLines: Int

The maximum number of lines a wrapping text field displays before clipping or truncating the text.

