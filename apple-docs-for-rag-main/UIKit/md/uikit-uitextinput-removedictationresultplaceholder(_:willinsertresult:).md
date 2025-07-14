

- UIKit
- UITextInput
-  removeDictationResultPlaceholder(\_:willInsertResult:) 

Instance Method

# removeDictationResultPlaceholder(\_:willInsertResult:)

Tells the view that the specified placeholder object is unnecessary.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func removeDictationResultPlaceholder(
    _ placeholder: Any,
    willInsertResult: Bool
)
```

## Parameters 

`placeholder`  

The placeholder object that is no longer needed.

`willInsertResult`  

The value of this parameter is true if the dictation value was generated successfully or false if an error occurred.

## Discussion

If the value in the `willInsertResult` parameter is false, the placeholder animation is not replaced by an actual dictation result. When this happens, the system still removes the placeholder animation and removes the strong reference to your placeholder object.

Important

This method is called only if the custom text view client leverages system selection by subclassing `UITextView`. Other clients can use dictationRecordingDidEnd() and dictationRecognitionFailed() to implement a custom placeholder.

## See Also

### Using dictation

func dictationRecordingDidEnd()

Tells the object when there is a pending dictation result.

func dictationRecognitionFailed()

Tells the object when dictation ends, but recognition fails.

func insertDictationResult([UIDictationPhrase])

Tells the object when there is more than one interpretation of a spoken phrase in a dictation result.

var insertDictationResultPlaceholder: Any

Asks for the placeholder object to use while generating dictation results.

func frame(forDictationResultPlaceholder: Any) -> CGRect

Asks for the rectangle for displaying the dictation placeholder animation.

