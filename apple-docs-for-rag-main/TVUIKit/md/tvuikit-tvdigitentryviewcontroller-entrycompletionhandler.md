

- TVUIKit
- TVDigitEntryViewController
-  entryCompletionHandler 

Instance Property

# entryCompletionHandler

A completion handler that cues the app that the user has entered the required number of digits for the digit entry view.

tvOS 12.0+

``` source
@MainActor
var entryCompletionHandler: (String) -> Void { get set }
```

## Parameters 

`entry`  

The digits that the user entered into the digit entry view.

## Discussion

Your app should respond with any required actions in response to the user’s entry.

## See Also

### Entering Information

func clearEntry(animated: Bool)

Removes all digits from the digit entry view.

