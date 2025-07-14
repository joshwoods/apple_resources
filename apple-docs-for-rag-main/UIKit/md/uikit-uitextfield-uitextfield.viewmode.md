

- UIKit
- UITextField
-  UITextField.ViewMode 

Enumeration

# UITextField.ViewMode

Constants that define when overlay views appear in a text field.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ViewMode
```

## Topics

### Constants

case never

The overlay view never appears.

case whileEditing

The overlay view is displayed only while text is being edited in the text field.

case unlessEditing

The overlay view is displayed only when text is not being edited.

case always

The overlay view is always displayed if the text field contains text.

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

### Managing overlay views

var clearButtonMode: UITextField.ViewMode

A mode that controls when the standard Clear button appears in the text field.

var leftView: UIView?

The overlay view that displays on the left (or leading) side of the text field.

var leftViewMode: UITextField.ViewMode

A mode that controls when the left overlay view appears in the text field.

var rightView: UIView?

The overlay view that displays on the right (or trailing) side of the text field.

var rightViewMode: UITextField.ViewMode

A mode that controls when the right overlay view appears in the text field.

