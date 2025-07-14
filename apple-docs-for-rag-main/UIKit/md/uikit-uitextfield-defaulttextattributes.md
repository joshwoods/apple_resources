

- UIKit
- UITextField
-  defaultTextAttributes 

Instance Property

# defaultTextAttributes

The default attributes to apply to the text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var defaultTextAttributes: [NSAttributedString.Key : Any] { get set }
```

## Discussion

By default, this property returns a dictionary of text attributes with default values.

Setting this property applies the specified attributes to the entire text of the text field. Unset attributes maintain their default values.

Getting this property returns the previously set attributes, which may have been modified by setting properties such as font and textColor.

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

