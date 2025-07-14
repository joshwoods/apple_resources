

- AppKit
- NSSpeechRecognizer
-  startListening() 

Instance Method

# startListening()

Tells the speech recognition engine to begin listening for commands.

macOS

``` source
func startListening()
```

## Discussion

When a command is recognized the message speechRecognizer(_:didRecognizeCommand:) is sent to the delegate.

## See Also

### Listening

func stopListening()

Tells the speech recognition engine to suspend listening for commands.

