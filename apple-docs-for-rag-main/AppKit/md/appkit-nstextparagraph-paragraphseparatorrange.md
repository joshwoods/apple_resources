

- AppKit
- NSTextParagraph
-  paragraphSeparatorRange 

Instance Property

# paragraphSeparatorRange

Returns the range of the paragraph separator in the containing text’s attributed string.

macOS 12.0+

``` source
var paragraphSeparatorRange: NSTextRange? { get }
```

## Discussion

The containing text is NSTextContentStorage’s attributedString.

## See Also

### Getting paragraph characteristics

var attributedString: NSAttributedString

Returns the source attributed string.

var paragraphContentRange: NSTextRange?

Returns the range of the paragraph in the containing text’s attributed string.

