

- UIKit
- UITextField
-  leftViewMode 

Instance Property

# leftViewMode

A mode that controls when the left overlay view appears in the text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var leftViewMode: UITextField.ViewMode { get set }
```

## Discussion

The default value for this property is UITextField.ViewMode.never. Note that the left overlay view flips automatically in a right-to-left user interface.

## See Also

### Managing overlay views

var clearButtonMode: UITextField.ViewMode

A mode that controls when the standard Clear button appears in the text field.

var leftView: UIView?

The overlay view that displays on the left (or leading) side of the text field.

var rightView: UIView?

The overlay view that displays on the right (or trailing) side of the text field.

var rightViewMode: UITextField.ViewMode

A mode that controls when the right overlay view appears in the text field.

enum ViewMode

Constants that define when overlay views appear in a text field.

