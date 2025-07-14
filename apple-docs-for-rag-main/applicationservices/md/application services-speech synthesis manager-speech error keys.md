

- Application Services
- Speech Synthesis Manager
-  Speech Error Keys 

API Collection

# Speech Error Keys

Keys used with the `kSpeechErrorsProperty` property to describe errors encountered during speech processing and production.

## Topics

### Constants

let kSpeechErrorCount: CFString

The number of errors that have occurred in processing the current text string, since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

let kSpeechErrorOldest: CFString

The error code of the first error that occurred since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

let kSpeechErrorOldestCharacterOffset: CFString

The position in the text string of the first error that occurred since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

let kSpeechErrorNewest: CFString

The error code of the most recent error that occurred since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

let kSpeechErrorNewestCharacterOffset: CFString

The position in the text string of the most recent error that occurred since the last call to the CopySpeechProperty(_:_:_:) function with the `kSpeechErrorsProperty` property.

