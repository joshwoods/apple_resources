

- UIKit
- UIInputViewController
-  advanceToNextInputMode() 

Instance Method

# advanceToNextInputMode()

Switches to the next keyboard in the list of user-enabled keyboards.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func advanceToNextInputMode()
```

## Discussion

When the user taps the Globe or a custom “next keyboard” key, the system picks the appropriate “next” keyboard from the list of user-enabled keyboards. To determine whether your custom keyboard needs to display a “next keyboard” key, check the needsInputModeSwitchKey property. If the value of the property is true, your keyboard should include this key.

## See Also

### Controlling a custom keyboard

func dismissKeyboard()

Dismisses the custom keyboard from the screen.

func handleInputModeList(from: UIView, with: UIEvent)

Supports interaction with the list of user-enabled keyboards.

