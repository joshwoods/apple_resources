

- Application Services
- Speech Synthesis Manager
-  SpeechWordCFProcPtr 

Type Alias

# SpeechWordCFProcPtr

Defines a pointer to a Core Foundation-based word callback function that is called by the Speech Synthesis Manager before it pronounces a word.

macOS 10.5+

``` source
typealias SpeechWordCFProcPtr = (SpeechChannel, SRefCon, CFString, CFRange) -> Void
```

## Parameters 

`chan`  

The speech channel that has finished processing input text.

`refCon`  

The reference constant associated with the speech channel.

`aString`  

A string containing the original text passed to the speech synthesizer in the SpeakCFString(_:_:_:) call.

`wordRange`  

The range of characters in `aString` that corresponds to the word.

## Discussion

A word callback function defined by the `SpeechWordCFProcPtr` is the Core Foundation-based equivalent of a word callback function defined by SpeechWordProcPtr. The Speech Synthesis Manager calls a speech channel’s word callback function just before it pronounces a word. You might use such a callback function, for example, to highlight the word about to be spoken in a window.

You can specify a word callback function by passing the `kSpeechWordCFCallBack` property to theSetSpeechProperty(_:_:_:) function.

## See Also

### Callbacks

typealias SpeechDoneProcPtr

Defines a pointer to a speech-done callback functionwhich is called when the Speech Synthesis Manager finishes speakinga buffer of text.

typealias SpeechErrorProcPtr

Defines a pointer to an error callback functionthat handles syntax errors within commands embedded in a text bufferbeing processed by the Speech Synthesis Manager.

typealias SpeechErrorCFProcPtr

Defines a pointer to an error callback function that handles syntax errors within commands embedded in a `CFString` object being processed by the Speech Synthesis Manager.

typealias SpeechPhonemeProcPtr

Defines a pointer to a phoneme callback functionthat is called by the Speech Synthesis Manager before it pronouncesa phoneme.

typealias SpeechSyncProcPtr

Defines a pointer to a synchronization callbackfunction that is called when the Speech Synthesis Manager encountersa synchronization command embedded in a text buffer.

typealias SpeechTextDoneProcPtr

Defines a pointer to a text-done callback functionthat is called when the Speech Synthesis Manager has finished processinga buffer of text.

typealias SpeechWordProcPtr

Defines a pointer to a word callback functionthat is called by the Speech Synthesis Manager before it pronouncesa word.

