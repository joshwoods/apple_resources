

- UIKit
- UITextView
-  textHighlightAttributes 

Instance Property

# textHighlightAttributes

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var textHighlightAttributes: [NSAttributedString.Key : Any]! { get set }
```

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

var linkTextAttributes: [NSAttributedString.Key : Any]!

The attributes to apply to links.

var borderStyle: UITextView.BorderStyle

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

enum BorderStyle

