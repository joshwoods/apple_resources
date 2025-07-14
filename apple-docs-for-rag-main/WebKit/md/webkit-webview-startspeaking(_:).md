

- WebKit
- WebView
-  startSpeaking(\_:) 

Instance Method

# startSpeaking(\_:)

An action method that starts speaking the selected text or all text if there’s no selection.

macOS

``` source
@MainActor
func startSpeaking(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

Speech continues asynchronously until the end of the text or until terminated by invoking the stopSpeaking(_:) method. This method behaves similar to the startSpeaking(_:) method in NSTextView.

## See Also

### Controlling Speakable Text

func stopSpeaking(Any?)

An action method that stops speaking that is in progress.

