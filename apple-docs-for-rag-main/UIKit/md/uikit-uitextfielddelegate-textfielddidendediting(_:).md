

- UIKit
- UITextFieldDelegate
-  textFieldDidEndEditing(\_:) 

Instance Method

# textFieldDidEndEditing(\_:)

Tells the delegate when editing stops for the specified text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textFieldDidEndEditing(_ textField: UITextField)
```

## Parameters 

`textField`  

The text field for which editing ended.

## Discussion

This method is called after the text field resigns its first responder status. You can use this method to update your delegate’s state information. For example, you might use this method to hide overlay views that should be visible only while editing.

Implementation of this method by the delegate is optional. If your delegate also implements the textFieldDidEndEditing(_:reason:) method, UIKit calls that method in preference to this one.

## See Also

### Managing editing

func textFieldShouldBeginEditing(UITextField) -> Bool

Asks the delegate whether to begin editing in the specified text field.

func textFieldDidBeginEditing(UITextField)

Tells the delegate when editing begins in the specified text field.

func textFieldShouldEndEditing(UITextField) -> Bool

Asks the delegate whether to stop editing in the specified text field.

func textFieldDidEndEditing(UITextField, reason: UITextField.DidEndEditingReason)

Tells the delegate when editing stops for the specified text field, and the reason it stopped.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

