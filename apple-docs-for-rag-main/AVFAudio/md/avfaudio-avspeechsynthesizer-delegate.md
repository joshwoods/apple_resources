

- AVFAudio
- AVSpeechSynthesizer
-  delegate 

Instance Property

# delegate

The delegate object for the speech synthesizer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any AVSpeechSynthesizerDelegate)? { get set }
```

## See Also

### Managing the delegate

protocol AVSpeechSynthesizerDelegate

A delegate protocol that contains optional methods you can implement to respond to events that occur during speech synthesis.

