

- UIKit
- UITextFieldDelegate
-  textFieldShouldClear(\_:) 

Instance Method

# textFieldShouldClear(\_:)

Asks the delegate whether to remove the text field’s current contents.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textFieldShouldClear(_ textField: UITextField) -> Bool
```

## Parameters 

`textField`  

The text field containing the text.

## Return Value

true if the text field’s contents should be cleared; otherwise, false.

## Discussion

The text field calls this method in response to the user pressing the built-in clear button. (This button is not shown by default but can be enabled by changing the value in the clearButtonMode property of the text field.) This method is also called when editing begins and the clearsOnBeginEditing property of the text field is set to true.

If you do not implement this method, the text field clears the text as if the method had returned true.

## See Also

### Editing the text field’s text

func textField(UITextField, shouldChangeCharactersIn: NSRange, replacementString: String) -> Bool

Asks the delegate whether to change the specified text.

func textFieldShouldReturn(UITextField) -> Bool

Asks the delegate whether to process the pressing of the Return button for the text field.

