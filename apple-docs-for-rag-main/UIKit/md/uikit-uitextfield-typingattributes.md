

- UIKit
- UITextField
-  typingAttributes 

Instance Property

# typingAttributes

The attributes to apply to new text that the user enters.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var typingAttributes: [NSAttributedString.Key : Any]? { get set }
```

## Discussion

This dictionary contains the attribute keys (and corresponding values) to apply to newly typed text. When the text field’s selection changes, the contents of the dictionary are cleared automatically.

If the text field is not in editing mode, this property contains the value `nil`. Similarly, you cannot assign a value to this property unless the text field is currently in editing mode.

## See Also

### Related Documentation

var isEditing: Bool

A Boolean value that indicates whether the text field is currently in edit mode.

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

enum BorderStyle

The type of border around the text field.

