

- UIKit
- UITextFieldDelegate
-  textField(\_:insertInputSuggestion:) 

Instance Method

# textField(\_:insertInputSuggestion:)

Tells the delegate when the keyboard delivers an input suggestion.

iOS 18.4+iPadOS 18.4+

``` source
@MainActor
optional func textField(
    _ textField: UITextField,
    insertInputSuggestion inputSuggestion: UIInputSuggestion
)
```

## Parameters 

`textField`  

The text field that is currently the first responder.

`inputSuggestion`  

The input suggestion that the user or system selected.

## Mentioned in 

Adopting Smart Reply in your messaging or email app

