

- UIKit
- UITextView
-  font 

Instance Property

# font

The font of the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var font: UIFont? { get set }
```

## Discussion

This property applies to the entire text string. The default value of this property is the body style of the system font.

Note

You can get information about the fonts available on the system using the methods of the UIFont class.

In iOS 6 and later, assigning a new value to this property causes the new font to be applied to the entire contents of the text view. If you want to apply the font to only a portion of the text, you must create a new attributed string with the desired style information and assign it to the attributedText property.

## See Also

### Configuring appearance attributes

var textColor: UIColor?

The color of the text.

var textAlignment: NSTextAlignment

The technique for aligning the text.

var typingAttributes: [NSAttributedString.Key : Any]

The attributes to apply to new text that the user enters.

var linkTextAttributes: [NSAttributedString.Key : Any]!

The attributes to apply to links.

var borderStyle: UITextView.BorderStyle

var textHighlightAttributes: [NSAttributedString.Key : Any]!

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

enum BorderStyle

