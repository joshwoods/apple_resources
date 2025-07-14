

- UIKit
- UITextField
-  UITextField.BorderStyle 

Enumeration

# UITextField.BorderStyle

The type of border around the text field.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum BorderStyle
```

## Topics

### Constants

case none

The text field does not display a border.

case line

Displays a thin rectangle around the text field.

case bezel

Displays a bezel-style border for the text field. This style is typically used for standard data-entry fields.

case roundedRect

Displays a rounded-style border for the text field.

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

### Configuring the text attributes

var text: String?

The text that the text field displays.

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

