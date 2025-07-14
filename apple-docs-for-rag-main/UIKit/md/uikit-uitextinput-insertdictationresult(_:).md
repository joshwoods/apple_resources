

- UIKit
- UITextInput
-  insertDictationResult(\_:) 

Instance Method

# insertDictationResult(\_:)

Tells the object when there is more than one interpretation of a spoken phrase in a dictation result.

iOS 5.1+iPadOS 5.1+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func insertDictationResult(_ dictationResult: [UIDictationPhrase])
```

## Parameters 

`dictationResult`  

An array of UIDictationPhrase objects.

## Discussion

Implement this optional method if you want to support dictation phrase alternatives. If you do not implement this method, iOS inserts the most likely interpretation of the dictated phrase.

Important

This method is called only if the custom text view client leverages system selection by subclassing `UITextView`. Other clients can use dictationRecordingDidEnd() and dictationRecognitionFailed() to implement a custom placeholder.

## See Also

### Using dictation

func dictationRecordingDidEnd()

Tells the object when there is a pending dictation result.

func dictationRecognitionFailed()

Tells the object when dictation ends, but recognition fails.

var insertDictationResultPlaceholder: Any

Asks for the placeholder object to use while generating dictation results.

func frame(forDictationResultPlaceholder: Any) -> CGRect

Asks for the rectangle for displaying the dictation placeholder animation.

func removeDictationResultPlaceholder(Any, willInsertResult: Bool)

Tells the view that the specified placeholder object is unnecessary.

