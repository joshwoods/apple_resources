

- UIKit
- UITextView
-  UITextView.BorderStyle 

Enumeration

# UITextView.BorderStyle

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
enum BorderStyle
```

## Topics

### Enumeration Cases

case none

case roundedRect

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var textHighlightAttributes: [NSAttributedString.Key : Any]!

func drawTextHighlightBackground(for: NSTextRange, origin: CGPoint)

