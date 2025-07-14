

- UIKit
- UILabel
-  textAlignment 

Instance Property

# textAlignment

The technique for aligning the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textAlignment: NSTextAlignment { get set }
```

## Discussion

If you’re using styled text, assigning a new value to this property applies the text alignment to the entirety of the string in the attributedText property. If you want to apply the alignment to only a portion of the text, create a new attributed string with the desired style information and associate it with the label. If you aren’t using styled text, this property applies to the entire text string in the text property.

In iOS 9 and later, the default value of this property is NSTextAlignment.natural; prior to iOS 9, the default value was NSTextAlignment.left.

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

