

- UIKit
- UITextField
-  text 

Instance Property

# text

The text that the text field displays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var text: String? { get set }
```

## Discussion

Assigning a new value to this property also replaces the value of the attributedText property with the same text, albeit without any inherent style attributes. Instead the text view styles the new string using the font, textColor, and other style-related properties of the class.

This value is `nil` by default.

## See Also

### Configuring the text attributes

var attributedText: NSAttributedString?

The styled text that the text field displays.

var placeholder: String?

The string that displays when there is no other text in the text field.

var attributedPlaceholder: NSAttributedString?

The styled string that displays when there is no other text in the text field.

var defaultTextAttributes: [NSAttributedString.Key : Any]

The default attributes to apply to the text.

var font: UIFont?

The font of the text.

var textColor: UIColor?

The color of the text.

var textAlignment: NSTextAlignment

The technique for aligning the text.

var typingAttributes: [NSAttributedString.Key : Any]?

The attributes to apply to new text that the user enters.

enum BorderStyle

The type of border around the text field.

