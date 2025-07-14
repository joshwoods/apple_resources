

- Application Services
- Speech Synthesis Manager
-  SpeechStatusInfo 

Structure

# SpeechStatusInfo

Defines a speech status information structure, which stores information about the status of a speech channel.

macOS 10.0+

``` source
struct SpeechStatusInfo
```

## Overview

By calling the GetSpeechInfo function with the `soStatus` selector, you can find out information about the status of a speech channel.

## Topics

### Initializers

init()

init(outputBusy: DarwinBoolean, outputPaused: DarwinBoolean, inputBytesLeft: Int, phonemeCode: Int16)

### Instance Properties

var inputBytesLeft: Int

The number of input bytes of the text that the speech channel must still process. When `inputBytesLeft` is 0, the buffer of input text passed to one of the `SpeakText` or `SpeakBuffer` functions may be disposed of. When you call the `SpeakString` function, the Speech Synthesis Manager stores a duplicate of the string to be spoken in an internal buffer; thus, you may delete the original string immediately after calling `SpeakString`.

var outputBusy: DarwinBoolean

Whether the speech channel is currently producing speech. A speech channel is considered to be producing speech even at some times when no audio data is being produced through the Macintosh speaker. This occurs, for example, when the Speech Synthesis Manager is processing an input buffer but has not yet initiated speech or when speech output is paused.

var outputPaused: DarwinBoolean

Whether speech output in the speech channel has been paused by a call to the PauseSpeechAt(_:_:) function.

var phonemeCode: Int16

The opcode for the phoneme that the speech channel is currently processing.

