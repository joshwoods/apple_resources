

- UIKit
- UIInputViewController
-  dismissKeyboard() 

Instance Method

# dismissKeyboard()

Dismisses the custom keyboard from the screen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dismissKeyboard()
```

## Mentioned in 

Configuring a custom keyboard interface

## Discussion

Because a custom keyboard does not have access to the current text input object, you cannot send it a resignFirstResponder() message (as you would to dismiss the system keyboard when you are developing an app with text entry). To dismiss the custom keyboard, call dismissKeyboard() instead.

## See Also

### Controlling a custom keyboard

func advanceToNextInputMode()

Switches to the next keyboard in the list of user-enabled keyboards.

func handleInputModeList(from: UIView, with: UIEvent)

Supports interaction with the list of user-enabled keyboards.

