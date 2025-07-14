

- UIKit
- UILabel
-  lineBreakStrategy 

Instance Property

# lineBreakStrategy

The strategy that the system uses to break lines when laying out multiple lines of text.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy { get set }
```

## Discussion

The default value is standard.

Note

When the label has an attributed string value, the system ignores the textColor, font, textAlignment, lineBreakMode, and lineBreakStrategy properties. Set the foregroundColor (Swift)/NSForegroundColorAttributeName (Objective-C), font (Swift)/NSFontAttributeName (Objective-C), alignment, lineBreakMode, and lineBreakStrategy properties in the attributed string instead.

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

var isEnabled: Bool

A Boolean value that determines whether the label draws its text in an enabled state.

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

