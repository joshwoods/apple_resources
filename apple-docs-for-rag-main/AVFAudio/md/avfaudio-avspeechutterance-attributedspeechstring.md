

- AVFAudio
- AVSpeechUtterance
-  attributedSpeechString 

Instance Property

# attributedSpeechString

An attributed string that contains the text for speech synthesis.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var attributedSpeechString: NSAttributedString { get }
```

## Discussion

You can’t change an utterance’s text after initializaiton. If you want the speech synthesizer to speak different text, create a new utterance.

## See Also

### Inspecting utterance text

var speechString: String

A string that contains the text for speech synthesis.

