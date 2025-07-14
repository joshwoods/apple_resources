

- UIKit
- UITextView
-  linkTextAttributes 

Instance Property

# linkTextAttributes

The attributes to apply to links.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var linkTextAttributes: [NSAttributedString.Key : Any]! { get set }
```

## Discussion

The default attributes specify blue text with a single underline and the pointing hand cursor.

## See Also

### Configuring appearance attributes

var font: UIFont?

The font of the text.

var textColor: UIColor?

The color of the text.

var textAlignment: NSTextAlignment

The technique for aligning the text.

var typingAttributes: [NSAttributedString.Key : Any]

The attributes to apply to new text that the user enters.

var borderStyle: UITextView.BorderStyle

var textHighlightAttributes: [NSAttributedString.Key : Any]!

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

enum BorderStyle

