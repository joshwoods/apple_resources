

- Application Services
- Speech Synthesis Manager
-  Error Callback User-Information String 

API Collection

# Error Callback User-Information String

Specifies information about the text being synthesized when an error occurs.

## Topics

### Constants

let kSpeechErrorCallbackSpokenString: CFString

The text being synthesized when the error occurred.

let kSpeechErrorCallbackCharacterOffset: CFString

The character index in the text being synthesized when the error occurred (the string representing the text is in kSpeechErrorCallbackSpokenString).

