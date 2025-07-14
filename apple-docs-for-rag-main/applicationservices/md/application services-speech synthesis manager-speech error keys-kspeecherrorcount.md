

- Application Services
- Speech Synthesis Manager
- Speech Error Keys
-  kSpeechErrorCount 

Global Variable

# kSpeechErrorCount

The number of errors that have occurred in processing the current text string, since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

macOS 10.5+

``` source
let kSpeechErrorCount: CFString
```

## Discussion

Using the `kSpeechErrorOldest` keys and the `kSpeechErrorNewest` keys, you can get information about the oldest and most recent errors that occurred since the last call to CopySpeechProperty(_:_:_:), but you cannot get information about any intervening errors.

