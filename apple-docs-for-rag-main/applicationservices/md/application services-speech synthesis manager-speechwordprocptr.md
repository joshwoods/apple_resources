

- Application Services
- Speech Synthesis Manager
-  SpeechWordProcPtr 

Type Alias

# SpeechWordProcPtr

Defines a pointer to a word callback functionthat is called by the Speech Synthesis Manager before it pronouncesa word.

macOS 10.0+

``` source
typealias SpeechWordProcPtr = (SpeechChannel, SRefCon, UInt, UInt16) -> Void
```

## Parameters 

`chan`  

The speech channel that has finished processing input text.

`refCon`  

The reference constant associated with the speech channel.

`wordPos`  

The number of bytes between the beginning of the text buffer and the beginning of the word about to be pronounced.

`wordLen`  

The length in bytes of the word about to be pronounced.

## Discussion

The Speech Synthesis Manager calls a speech channel’s wordcallback function just before it pronounces a word. You might usesuch a callback function, for example, to draw the word about tobe spoken in a window. In this case, the callback function wouldset a global flag variable to indicate that the word being spokenis changing and another two global variables to `wordPos` and `wordLen`.A function called by your application’s main event loop coulddetect that the word being spoken is changing and draw the wordin a window.

You can specify a word callback function by passing the `soWordCallBack` selectorto the `SetSpeechInfo` function.

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

typealias SpeechWordCFProcPtr

Defines a pointer to a Core Foundation-based word callback function that is called by the Speech Synthesis Manager before it pronounces a word.

