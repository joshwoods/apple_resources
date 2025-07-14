

- UIKit
- UITextView
-  typingAttributes 

Instance Property

# typingAttributes

The attributes to apply to new text that the user enters.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var typingAttributes: [NSAttributedString.Key : Any] { get set }
```

## Discussion

This dictionary contains the attribute keys (and corresponding values) to apply to newly typed text. When the text view’s selection changes, the contents of the dictionary are cleared automatically.

## See Also

### Related Documentation

var isEditable: Bool

A Boolean value that indicates whether the text view is editable.

### Configuring appearance attributes

var font: UIFont?

The font of the text.

var textColor: UIColor?

The color of the text.

var textAlignment: NSTextAlignment

The technique for aligning the text.

var linkTextAttributes: [NSAttributedString.Key : Any]!

The attributes to apply to links.

var borderStyle: UITextView.BorderStyle

var textHighlightAttributes: [NSAttributedString.Key : Any]!

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

enum BorderStyle

