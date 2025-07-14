

- UIKit
- UITextView
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

This property applies to the entire text string. The default value of this property is NSTextAlignment.natural.

Assigning a new value to this property causes the new text alignment to be applied to the entire contents of the text view. If you want to apply the alignment to only a portion of the text, you must create a new attributed string with the desired style information and assign it to the attributedText property.

## See Also

### Configuring appearance attributes

var font: UIFont?

The font of the text.

var textColor: UIColor?

The color of the text.

var typingAttributes: [NSAttributedString.Key : Any]

The attributes to apply to new text that the user enters.

var linkTextAttributes: [NSAttributedString.Key : Any]!

The attributes to apply to links.

var borderStyle: UITextView.BorderStyle

var textHighlightAttributes: [NSAttributedString.Key : Any]!

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

enum BorderStyle

