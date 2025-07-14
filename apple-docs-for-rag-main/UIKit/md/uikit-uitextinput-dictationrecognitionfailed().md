

- UIKit
- UITextInput
-  dictationRecognitionFailed() 

Instance Method

# dictationRecognitionFailed()

Tells the object when dictation ends, but recognition fails.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func dictationRecognitionFailed()
```

## Discussion

Implement this optional method if you want to respond to failed dictation recognition.

## See Also

### Using dictation

func dictationRecordingDidEnd()

Tells the object when there is a pending dictation result.

func insertDictationResult([UIDictationPhrase])

Tells the object when there is more than one interpretation of a spoken phrase in a dictation result.

var insertDictationResultPlaceholder: Any

Asks for the placeholder object to use while generating dictation results.

func frame(forDictationResultPlaceholder: Any) -> CGRect

Asks for the rectangle for displaying the dictation placeholder animation.

func removeDictationResultPlaceholder(Any, willInsertResult: Bool)

Tells the view that the specified placeholder object is unnecessary.

