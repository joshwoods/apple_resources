

- AppKit
- NSSpeechRecognizer
-  delegate 

Instance Property

# delegate

The delegate for the speech recognizer object.

macOS

``` source
weak var delegate: (any NSSpeechRecognizerDelegate)? { get set }
```

## Discussion

The delegate must conform to the NSSpeechRecognizerDelegate protocol.

## See Also

### Handling the Recognition of a Spoken Command

protocol NSSpeechRecognizerDelegate

A set of optional methods implemented by delegates of NSSpeechRecognizer objects.

