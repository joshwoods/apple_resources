

- UIKit
- UITextFieldDelegate
-  textFieldShouldEndEditing(\_:) 

Instance Method

# textFieldShouldEndEditing(\_:)

Asks the delegate whether to stop editing in the specified text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textFieldShouldEndEditing(_ textField: UITextField) -> Bool
```

## Parameters 

`textField`  

The text field in which editing is about to end.

## Return Value

true if editing should stop or false if it should continue.

## Discussion

The text field calls this method when it is asked to resign the first responder status. This can happen when the user selects another control or when you call the text field’s resignFirstResponder() method. Before the focus change occurs, however, the text field calls this method and gives you a chance to prevent the change from happening.

Normally, you would return true from this method to allow the text field to resign the first responder status. You might return false, however, in cases where your delegate detects invalid contents in the text field. Returning false prevents the user from switching to another control until the text field contains a valid value.

Note

If you use this method to validate the contents of the text field, you might also want to use an overlay view to provide feedback to that effect. For example, you might display a small icon indicating the text is invalid. For more information about adding overlays to text fields, see the methods of UITextField.

Be aware that this method provides only a recommendation about whether editing should end. Even if you return false, UIKit might still force an end to editing. For example, text fields always resign the first responder status when they are removed from their parent view or window.

Implementation of this method by the delegate is optional. If you do not implement this method, the text field resigns the first responder status as if this method had returned true.

## See Also

### Managing editing

func textFieldShouldBeginEditing(UITextField) -> Bool

Asks the delegate whether to begin editing in the specified text field.

func textFieldDidBeginEditing(UITextField)

Tells the delegate when editing begins in the specified text field.

func textFieldDidEndEditing(UITextField, reason: UITextField.DidEndEditingReason)

Tells the delegate when editing stops for the specified text field, and the reason it stopped.

func textFieldDidEndEditing(UITextField)

Tells the delegate when editing stops for the specified text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

