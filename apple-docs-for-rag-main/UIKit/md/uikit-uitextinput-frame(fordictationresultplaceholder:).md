

- UIKit
- UITextInput
-  frame(forDictationResultPlaceholder:) 

Instance Method

# frame(forDictationResultPlaceholder:)

Asks for the rectangle for displaying the dictation placeholder animation.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func frame(forDictationResultPlaceholder placeholder: Any) -> CGRect
```

## Parameters 

`placeholder`  

A placeholder object provided by your app and used to identify the location of the dictation results.

## Return Value

The rectangle, in the coordinate system of your input view, at which to display the dictation placeholder animation.

## Discussion

While dictation results are being generated, UIKit displays the built-in dictation placeholder animation. Your implementation of this method should provide the rectangle at which to display this animation (at the location where the dictation results will be inserted).

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

func removeDictationResultPlaceholder(Any, willInsertResult: Bool)

Tells the view that the specified placeholder object is unnecessary.

