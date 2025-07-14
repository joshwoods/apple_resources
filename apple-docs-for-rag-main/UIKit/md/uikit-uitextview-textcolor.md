

- UIKit
- UITextView
-  textColor 

Instance Property

# textColor

The color of the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textColor: UIColor? { get set }
```

## Discussion

This property applies to the entire text string. The default text color is black.

In iOS 6 and later, assigning a new value to this property causes the new text color to be applied to the entire contents of the text view. If you want to apply the color to only a portion of the text, you must create a new attributed string with the desired style information and assign it to the attributedText property.

## See Also

### Related Documentation

var backgroundColor: UIColor?

The view’s background color.

### Configuring appearance attributes

var font: UIFont?

The font of the text.

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

