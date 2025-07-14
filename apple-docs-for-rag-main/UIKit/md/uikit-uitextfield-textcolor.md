

- UIKit
- UITextField
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

This property applies to the entire text string. The default value for this property is a black color. The value for the property can only be set to a non-`nil` value; setting this property to `nil` raises an exception.

If you are using styled text, assigning a new value to this property causes the text color to be applied to the entire string in the attributedText property. If you want to apply the color to only a portion of the text, create a new attributed string with the desired style information and associate it with the text field.

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

var textAlignment: NSTextAlignment

The technique for aligning the text.

var typingAttributes: [NSAttributedString.Key : Any]?

The attributes to apply to new text that the user enters.

enum BorderStyle

The type of border around the text field.

