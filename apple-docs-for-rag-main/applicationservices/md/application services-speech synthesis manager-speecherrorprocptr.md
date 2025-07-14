

- Application Services
- Speech Synthesis Manager
-  SpeechErrorProcPtr 

Type Alias

# SpeechErrorProcPtr

Defines a pointer to an error callback functionthat handles syntax errors within commands embedded in a text bufferbeing processed by the Speech Synthesis Manager.

macOS 10.0+

``` source
typealias SpeechErrorProcPtr = (SpeechChannel, SRefCon, OSErr, Int) -> Void
```

## Parameters 

`chan`  

The speech channel that has finished processing input text.

`refCon`  

The reference constant associated with the speech channel.

`theError`  

The error that occurred in processing an embedded command.

`bytePos`  

The number of bytes from the beginning of the text buffer being spoken to the error encountered.

## Discussion

The Speech Synthesis Manager calls a speech channel’s errorcallback function whenever it encounters a syntax error within acommand embedded in a text buffer it is processing. This can beuseful during application debugging, to detect problems with commandsthat you have embedded in text buffers that your application speaks.It can also be useful if your application allows users to embedcommands within text buffers. Your application might display analert indicating that the Speech Synthesis Manager encountered a problemin processing an embedded command.

Ordinarily, the error information that the Speech SynthesisManager provides the error callback function should be sufficient.However, if your application needs information about errors thatoccurred before the error callback function was enabled, the application (includingthe error callback function) can call the `GetSpeechInfo` functionwith the `soErrors` selector.

You can specify an error callback function by passing the `soErrorCallBack` selectorto the `SetSpeechInfo` function.

## See Also

### Callbacks

typealias SpeechDoneProcPtr

Defines a pointer to a speech-done callback functionwhich is called when the Speech Synthesis Manager finishes speakinga buffer of text.

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

typealias SpeechWordCFProcPtr

Defines a pointer to a Core Foundation-based word callback function that is called by the Speech Synthesis Manager before it pronounces a word.

