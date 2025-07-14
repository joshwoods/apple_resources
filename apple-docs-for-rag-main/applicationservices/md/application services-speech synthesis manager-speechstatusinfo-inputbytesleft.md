

- Application Services
- Speech Synthesis Manager
- SpeechStatusInfo
-  inputBytesLeft 

Instance Property

# inputBytesLeft

The number of input bytes of the text that the speech channel must still process. When `inputBytesLeft` is 0, the buffer of input text passed to one of the `SpeakText` or `SpeakBuffer` functions may be disposed of. When you call the `SpeakString` function, the Speech Synthesis Manager stores a duplicate of the string to be spoken in an internal buffer; thus, you may delete the original string immediately after calling `SpeakString`.

macOS 10.0+

``` source
var inputBytesLeft: Int
```

