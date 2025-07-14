

- AppKit
- NSSpeechRecognizerDelegate
-  speechRecognizer(\_:didRecognizeCommand:) 

Instance Method

# speechRecognizer(\_:didRecognizeCommand:)

Invoked when the recognition engine has recognized the application command `command`.

macOS

``` source
@MainActor
optional func speechRecognizer(
    _ sender: NSSpeechRecognizer,
    didRecognizeCommand command: String
)
```

## Discussion

`command` is one of the strings from the array passed to commands. The delegate typically evaluates which command was recognized and performs the related action.

## See Also

### Related Documentation

Speech Programming Topics

