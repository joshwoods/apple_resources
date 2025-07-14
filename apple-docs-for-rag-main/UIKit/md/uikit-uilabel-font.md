

- UIKit
- UILabel
-  font 

Instance Property

# font

The font of the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var font: UIFont! { get set }
```

## Discussion

If you’re using styled text, assigning a new value to this property applies the font to the entirety of the string in the attributedText property. If you want to apply the font to only a portion of the text, create a new attributed string with the desired style information and associate it with the label. If you aren’t using styled text, this property applies to the entire text string in the text property.

The default value for this property is the system font at a size of 17 points (using the systemFont(ofSize:) class method of UIFont). Setting this property to `nil` causes it to be reset to the default value.

## See Also

### Accessing the text attributes

var text: String?

The text that the label displays.

var attributedText: NSAttributedString?

The styled text that the label displays.

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

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

