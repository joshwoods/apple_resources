

- UIKit
- UITextFieldDelegate
-  textFieldDidBeginEditing(\_:) 

Instance Method

# textFieldDidBeginEditing(\_:)

Tells the delegate when editing begins in the specified text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textFieldDidBeginEditing(_ textField: UITextField)
```

## Parameters 

`textField`  

The text field in which an editing session began.

## Discussion

This method notifies the delegate that the specified text field just became the first responder. Use this method to update state information or perform other tasks. For example, you might use this method to show overlay views that are visible only while editing.

Implementation of this method by the delegate is optional.

## See Also

### Managing editing

func textFieldShouldBeginEditing(UITextField) -> Bool

Asks the delegate whether to begin editing in the specified text field.

func textFieldShouldEndEditing(UITextField) -> Bool

Asks the delegate whether to stop editing in the specified text field.

func textFieldDidEndEditing(UITextField, reason: UITextField.DidEndEditingReason)

Tells the delegate when editing stops for the specified text field, and the reason it stopped.

func textFieldDidEndEditing(UITextField)

Tells the delegate when editing stops for the specified text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

