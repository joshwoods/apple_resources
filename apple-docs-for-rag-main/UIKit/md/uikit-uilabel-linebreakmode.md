

- UIKit
- UILabel
-  lineBreakMode 

Instance Property

# lineBreakMode

The technique for wrapping and truncating the label’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var lineBreakMode: NSLineBreakMode { get set }
```

## Discussion

If you aren’t using styled text, this property applies to the entire text string in the text property. If you’re using styled text, assigning a new value to this property applies the line break mode to the entirety of the string in the attributedText property. To apply the line break mode to only a portion of the text, create a new attributed string with the desired style information and associate it with the label. However, NSParagraphStyle properties, such as those defined by NSLineBreakMode, apply to entire paragraphs (as defined for paragraphRange(for:)), not words within paragraphs.

This property is in effect both during normal drawing and in cases where the label must reduce the font size to fit the text in its bounding box. The default value of this property is NSLineBreakMode.byTruncatingTail.

## See Also

### Related Documentation

var adjustsFontSizeToFitWidth: Bool

A Boolean value that determines whether the label reduces the text’s font size to fit the title string into the label’s bounding rectangle.

### Accessing the text attributes

var text: String?

The text that the label displays.

var attributedText: NSAttributedString?

The styled text that the label displays.

var font: UIFont!

The font of the text.

var textColor: UIColor!

The color of the text.

var textAlignment: NSTextAlignment

The technique for aligning the text.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

var isEnabled: Bool

A Boolean value that determines whether the label draws its text in an enabled state.

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

