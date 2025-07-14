

- UIKit
- UILabel
-  attributedText 

Instance Property

# attributedText

The styled text that the label displays.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@NSCopying @MainActor
var attributedText: NSAttributedString? { get set }
```

## Discussion

This property is `nil` by default.

Assigning a new value to this property also replaces the value of the text property with the same string data, although without any formatting information. In addition, assigning a new value updates the values in the font, textColor, and other style-related properties so that they reflect the style information starting at location `0` in the attributed string.

Turn autokerning on for the label by setting the kern (Swift) or NSKernAttributeName (Objective-C) of the string to doc://com.apple.documentation/documentation/foundation/nsnull/1520557-null.

## See Also

### Accessing the text attributes

var text: String?

The text that the label displays.

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

