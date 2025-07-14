

- WebKit
- WebView
-  showGuessPanel(\_:) 

Instance Method

# showGuessPanel(\_:)

An action method that shows a spelling correction panel.

macOS

``` source
@MainActor
func showGuessPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action method opens the Spelling panel, allowing the user to make a correction during spell checking.

## See Also

### Spell-checking Action Methods

func checkSpelling(Any?)

An action method that searches for a misspelled word in the receiver.

