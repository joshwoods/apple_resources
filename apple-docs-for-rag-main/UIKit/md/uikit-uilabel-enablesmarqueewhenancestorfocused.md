

- UIKit
- UILabel
-  enablesMarqueeWhenAncestorFocused 

Instance Property

# enablesMarqueeWhenAncestorFocused

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

tvOS 12.0+

``` source
@MainActor
var enablesMarqueeWhenAncestorFocused: Bool { get set }
```

## Discussion

If this value is true, then the label ignores lineBreakMode, adjustsFontSizeToFitWidth, and allowsDefaultTighteningForTruncation. The label scrolls its text when any ancestor in its view hierarchy has focus.

The default value for this property is false.

## See Also

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

var lineBreakMode: NSLineBreakMode

The technique for wrapping and truncating the label’s text.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

var isEnabled: Bool

A Boolean value that determines whether the label draws its text in an enabled state.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

