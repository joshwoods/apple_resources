

- UIKit
- UITextField
-  rightView 

Instance Property

# rightView

The overlay view that displays on the right (or trailing) side of the text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var rightView: UIView? { get set }
```

## Discussion

You can use the right overlay view to provide indicate additional features available for the text field. For example, you might display a bookmarks button in this location to allow the user to select from a set of predefined items. The right overlay view flips automatically in a right-to-left user interface.

The right overlay view is placed in the rectangle returned by the rightViewRect(forBounds:) method of the receiver. The image associated with this property should fit the given rectangle. If it does not fit, it is scaled to fit. If you specify a control for your view, that control tracks and sends actions as usual.

If your right overlay view overlaps a sibling view, such as the clear button, you must use the UITextField.ViewMode to implement proper behavior. For example, if clearButtonMode is set to display the clear button, you can set the right overlay view’s rightViewMode to UITextField.ViewMode.unlessEditing to reveal the clear button during editing when the text field has contents.

## See Also

### Related Documentation

func rightViewRect(forBounds: CGRect) -> CGRect

Returns the drawing location of the text field’s right overlay view.

### Managing overlay views

var clearButtonMode: UITextField.ViewMode

A mode that controls when the standard Clear button appears in the text field.

var leftView: UIView?

The overlay view that displays on the left (or leading) side of the text field.

var leftViewMode: UITextField.ViewMode

A mode that controls when the left overlay view appears in the text field.

var rightViewMode: UITextField.ViewMode

A mode that controls when the right overlay view appears in the text field.

enum ViewMode

Constants that define when overlay views appear in a text field.

