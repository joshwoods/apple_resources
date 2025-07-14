

- WatchKit
- WKInterfaceController
-  presentTextInputController(withSuggestions:allowedInputMode:completion:) 

Instance Method

# presentTextInputController(withSuggestions:allowedInputMode:completion:)

Displays a modal interface for gathering text input from the user.

watchOS 2.0+

``` source
@MainActor
func presentTextInputController(
    withSuggestions suggestions: [String]?,
    allowedInputMode inputMode: WKTextInputMode,
    completion: @escaping ([Any]?) -> Void
)
```

``` source
@MainActor
func presentTextInputController(
    withSuggestions suggestions: [String]?,
    allowedInputMode inputMode: WKTextInputMode
) async -> [Any]?
```

## Parameters 

`suggestions`  

An array of NSString objects, each of which contains a suggested phrase for input. The user can either select one of the phrases you suggest or input a new text phrase.

`inputMode`  

The type of input to allow. For a list of possible values, see WKTextInputMode.

`completion`  

The block to execute after the user dismisses the modal interface. This block has no return value and takes the following parameter:

results  
An array containing the input from the user, or `nil` if the user canceled the operation. When an array is provided, the value in the array is usually an NSString object representing the text input. The array can also contain an emoji image, packaged as an NSData object. You can use the data object to create a corresponding UIImage object.

## Mentioned in 

Navigating Between Scenes

## Discussion

This method executes asynchronously, returning shortly after you call it. During a subsequent run loop cycle, the system displays a text input controller to the user. The input controller displays the list of input phrases you specify and provides options to enter new text phrases through dictation or to select from a list of emoji.

When the user accepts a value or cancels input, the text input controller dismisses itself and then executes the block in the `completion` parameter on the WatchKit extension’s main thread. Use the block to retrieve the accepted value and apply it to your content. The presenting interface controller is activated before the block is executed.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Handling text input

func presentTextInputControllerWithSuggestions(forLanguage: ((String) -> [Any]?)?, allowedInputMode: WKTextInputMode, completion: ([Any]?) -> Void)

Displays a modal interface for gathering language-specific text input from the user.

func dismissTextInputController()

Dismisses the text input controller without returning any text.

enum WKTextInputMode

The input modes supported by the text input controller.

