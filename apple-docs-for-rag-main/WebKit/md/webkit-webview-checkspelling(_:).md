

- WebKit
- WebView
-  checkSpelling(\_:) 

Instance Method

# checkSpelling(\_:)

An action method that searches for a misspelled word in the receiver.

macOS

``` source
@MainActor
func checkSpelling(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action method starts a search at the end of the selection and continues until it reaches a word suspected of being misspelled or the end of the content. If a word isn’t recognized by the spelling server, a showGuessPanel(_:) message is sent to the receiver which opens the Guess panel and allows the user to make a correction or add the word to the local dictionary.

## See Also

### Spell-checking Action Methods

func showGuessPanel(Any?)

An action method that shows a spelling correction panel.

