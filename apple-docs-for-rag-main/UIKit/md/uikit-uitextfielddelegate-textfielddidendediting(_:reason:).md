

- UIKit
- UITextFieldDelegate
-  textFieldDidEndEditing(\_:reason:) 

Instance Method

# textFieldDidEndEditing(\_:reason:)

Tells the delegate when editing stops for the specified text field, and the reason it stopped.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional func textFieldDidEndEditing(
    _ textField: UITextField,
    reason: UITextField.DidEndEditingReason
)
```

## Parameters 

`textField`  

The text field for which editing ended.

`reason`  

The reason why editing ended. Use this field to determine whether to incorporate the text editing changes or abandon them.

## Discussion

This method is called after the text field resigns its first responder status. You can use this method to update your delegate’s state information. For example, you might use this method to hide overlay views that should be visible only while editing.

Implementation of this method by the delegate is optional. UIKit calls this method in preference to the textFieldDidEndEditing(_:) method.

## See Also

### Managing editing

func textFieldShouldBeginEditing(UITextField) -> Bool

Asks the delegate whether to begin editing in the specified text field.

func textFieldDidBeginEditing(UITextField)

Tells the delegate when editing begins in the specified text field.

func textFieldShouldEndEditing(UITextField) -> Bool

Asks the delegate whether to stop editing in the specified text field.

func textFieldDidEndEditing(UITextField)

Tells the delegate when editing stops for the specified text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

