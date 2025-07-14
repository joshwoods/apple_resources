

- UIKit
- UITextField
-  placeholder 

Instance Property

# placeholder

The string that displays when there is no other text in the text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var placeholder: String? { get set }
```

## Discussion

This value is `nil` by default. The placeholder string is drawn using a system-defined color.

## See Also

### Configuring the text attributes

var text: String?

The text that the text field displays.

var attributedText: NSAttributedString?

The styled text that the text field displays.

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

