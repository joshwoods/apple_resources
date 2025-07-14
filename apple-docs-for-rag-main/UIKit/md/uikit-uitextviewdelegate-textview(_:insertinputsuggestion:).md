

- UIKit
- UITextViewDelegate
-  textView(\_:insertInputSuggestion:) 

Instance Method

# textView(\_:insertInputSuggestion:)

Tells the delegate when the keyboard delivers an input suggestion.

iOS 18.4+iPadOS 18.4+

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    insertInputSuggestion inputSuggestion: UIInputSuggestion
)
```

## Parameters 

`textView`  

The text view that is currently the first responder.

`inputSuggestion`  

The input suggestion that the user or system selected.

## Mentioned in 

Adopting Smart Reply in your messaging or email app

