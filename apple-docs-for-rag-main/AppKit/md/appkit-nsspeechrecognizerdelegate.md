

- AppKit
-  NSSpeechRecognizerDelegate 

Protocol

# NSSpeechRecognizerDelegate

A set of optional methods implemented by delegates of NSSpeechRecognizer objects.

macOS

``` source
protocol NSSpeechRecognizerDelegate : NSObjectProtocol
```

## Topics

### Recognizing Commands

func speechRecognizer(NSSpeechRecognizer, didRecognizeCommand: String)

Invoked when the recognition engine has recognized the application command `command`.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling the Recognition of a Spoken Command

var delegate: (any NSSpeechRecognizerDelegate)?

The delegate for the speech recognizer object.

