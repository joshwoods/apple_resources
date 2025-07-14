

- UIKit
- UITextInput
-  insertDictationResultPlaceholder 

Instance Property

# insertDictationResultPlaceholder

Asks for the placeholder object to use while generating dictation results.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var insertDictationResultPlaceholder: Any { get }
```

## Return Value

A placeholder object to use to identify the dictation results. This value must not be `nil`.

## Discussion

Implementation of this method is optional but can be done when you want to provide a specific rectangle for the placeholder animation while the dictation results are being processed. The object you return from this method is passed to the frame(forDictationResultPlaceholder:) method later. The actual contents of the object are not accessed by UIKit but you can use the object to store whatever information you need to identify the location for the animation.

UIKit maintains a strong reference to your placeholder object until the removeDictationResultPlaceholder(_:willInsertResult:) method is called. You must implement both this method and the removeDictationResultPlaceholder(_:willInsertResult:) method for placeholders to be used.

## See Also

### Using dictation

func dictationRecordingDidEnd()

Tells the object when there is a pending dictation result.

func dictationRecognitionFailed()

Tells the object when dictation ends, but recognition fails.

func insertDictationResult([UIDictationPhrase])

Tells the object when there is more than one interpretation of a spoken phrase in a dictation result.

func frame(forDictationResultPlaceholder: Any) -> CGRect

Asks for the rectangle for displaying the dictation placeholder animation.

func removeDictationResultPlaceholder(Any, willInsertResult: Bool)

Tells the view that the specified placeholder object is unnecessary.

