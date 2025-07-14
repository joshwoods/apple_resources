

- UIKit
- UILabel
-  showsExpansionTextWhenTruncated 

Instance Property

# showsExpansionTextWhenTruncated

A Boolean value that determines whether the full text of the label displays when the pointer hovers over the truncated text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 15.0+tvOSvisionOS 1.0+

``` source
@MainActor
var showsExpansionTextWhenTruncated: Bool { get set }
```

## Discussion

A label may truncate text too long to fit in its container based on the value of the label’s lineBreakMode property. To provide the option in your app to show the full text when the pointer hovers over the truncated text, set showsExpansionTextWhenTruncated to true. The default value is false.

Note

Text expansion is available in iPhone and iPad apps running on a Mac with Apple silicon and in Mac apps built with Mac Catalyst.

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

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

