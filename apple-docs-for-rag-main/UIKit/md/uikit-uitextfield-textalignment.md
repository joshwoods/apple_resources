

- UIKit
- UITextField
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

This property applies to the both the main text string and the placeholder string. The default value of this property is NSLeftTextAlignment.

If you are using styled text, assigning a new value to this property causes the text alignment to be applied to the entire string in the attributedText property. If you want to apply the alignment to only a portion of the text, create a new attributed string with the desired style information and associate it with the text field.

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

var typingAttributes: [NSAttributedString.Key : Any]?

The attributes to apply to new text that the user enters.

enum BorderStyle

The type of border around the text field.

