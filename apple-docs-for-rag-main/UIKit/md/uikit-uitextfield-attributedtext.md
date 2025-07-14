

- UIKit
- UITextField
-  attributedText 

Instance Property

# attributedText

The styled text that the text field displays.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@NSCopying @MainActor
var attributedText: NSAttributedString? { get set }
```

## Discussion

This property is `nil` by default. Assigning a new value to this property also replaces the value of the text property with the same string data, albeit without any formatting information. In addition, assigning a new value updates the values in the font, textColor, and other style-related properties so that they reflect the style information starting at location `0` in the attributed string.

## See Also

### Configuring the text attributes

var text: String?

The text that the text field displays.

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

