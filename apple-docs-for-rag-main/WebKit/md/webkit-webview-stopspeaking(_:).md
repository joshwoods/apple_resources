

- WebKit
- WebView
-  stopSpeaking(\_:) 

Instance Method

# stopSpeaking(\_:)

An action method that stops speaking that is in progress.

macOS

``` source
@MainActor
func stopSpeaking(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action method stops speech that was previously started with startSpeaking(_:). This method behaves similar to the stopSpeaking(_:) method in NSTextView.

## See Also

### Controlling Speakable Text

func startSpeaking(Any?)

An action method that starts speaking the selected text or all text if there’s no selection.

