

- AppKit
- NSTextField
-  maximumNumberOfLines 

Instance Property

# maximumNumberOfLines

The maximum number of lines a wrapping text field displays before clipping or truncating the text.

macOS 10.11+

``` source
@MainActor
var maximumNumberOfLines: Int { get set }
```

## Discussion

The default value of `0` indicates no limit to the number of lines, and the text fills the bounds of the text field cell.

If the text field reaches the maximum number of lines, or if the height of the container can’t accommodate the number of lines, the text field clips or truncates the text, depending on the cell’s truncatesLastVisibleLine setting.

Important

This value also affects sizeThatFits(_:), fittingSize, and intrinsicContentSize. If the value of this property isn’t `1`, the text field may use multiple lines to determine its intrinsic content size.

## See Also

### Configuring Line Wrapping

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that controls whether single-line text fields tighten intercharacter spacing before truncating the text.

