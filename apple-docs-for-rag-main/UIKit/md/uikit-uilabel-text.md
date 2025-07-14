

- UIKit
- UILabel
-  text 

Instance Property

# text

The text that the label displays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var text: String? { get set }
```

## Discussion

This property is `nil` by default. Assigning a new value to this property also replaces the value of the attributedText property with the same text, although without any inherent style attributes. Instead the label styles the new string using shadowColor, textAlignment, and other style-related properties of the class.

## See Also

### Accessing the text attributes

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

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

