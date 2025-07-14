

- UIKit
- UITextFieldDelegate
-  textFieldShouldReturn(\_:) 

Instance Method

# textFieldShouldReturn(\_:)

Asks the delegate whether to process the pressing of the Return button for the text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func textFieldShouldReturn(_ textField: UITextField) -> Bool
```

## Parameters 

`textField`  

The text field whose return button was pressed.

## Return Value

true if the text field should implement its default behavior for the return button; otherwise, false.

## Discussion

The text field calls this method whenever the user taps the return button. You can use this method to implement any custom behavior when the button is tapped. For example, if you want to dismiss the keyboard when the user taps the return button, your implementation can call the resignFirstResponder() method.

## See Also

### Editing the text field’s text

func textField(UITextField, shouldChangeCharactersIn: NSRange, replacementString: String) -> Bool

Asks the delegate whether to change the specified text.

func textFieldShouldClear(UITextField) -> Bool

Asks the delegate whether to remove the text field’s current contents.

