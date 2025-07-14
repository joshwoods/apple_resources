

- UIKit
- UITextField
-  attributedPlaceholder 

Instance Property

# attributedPlaceholder

The styled string that displays when there is no other text in the text field.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@NSCopying @MainActor
var attributedPlaceholder: NSAttributedString? { get set }
```

## Discussion

This property is `nil` by default. If set, the placeholder string is drawn using system-defined color and the remaining style information (except the text color) of the attributed string. Assigning a new value to this property also replaces the value of the placeholder property with the same string data, albeit without any formatting information. Assigning a new value to this property does not affect any other style-related properties of the text field.

## See Also

### Configuring the text attributes

var text: String?

The text that the text field displays.

var attributedText: NSAttributedString?

The styled text that the text field displays.

var placeholder: String?

The string that displays when there is no other text in the text field.

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

