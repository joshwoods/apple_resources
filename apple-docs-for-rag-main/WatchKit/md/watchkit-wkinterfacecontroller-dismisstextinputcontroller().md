

- WatchKit
- WKInterfaceController
-  dismissTextInputController() 

Instance Method

# dismissTextInputController()

Dismisses the text input controller without returning any text.

watchOS 2.0+

``` source
@MainActor
func dismissTextInputController()
```

## Discussion

Use this method to cancel a text input operation without accepting any input from the user. Dismissing the interface controller animates it off the screen and does not call the associated completion block.

## See Also

### Handling text input

func presentTextInputController(withSuggestions: [String]?, allowedInputMode: WKTextInputMode, completion: ([Any]?) -> Void)

Displays a modal interface for gathering text input from the user.

func presentTextInputControllerWithSuggestions(forLanguage: ((String) -> [Any]?)?, allowedInputMode: WKTextInputMode, completion: ([Any]?) -> Void)

Displays a modal interface for gathering language-specific text input from the user.

enum WKTextInputMode

The input modes supported by the text input controller.

