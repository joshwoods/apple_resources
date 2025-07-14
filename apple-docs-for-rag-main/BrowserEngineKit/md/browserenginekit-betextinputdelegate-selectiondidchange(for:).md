

- BrowserEngineKit
- BETextInputDelegate
-  selectionDidChange(for:) 

Instance Method

# selectionDidChange(for:)

Tells the system when the selection has changed in the document.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
func selectionDidChange(for textInput: any BETextInput)
```

**Required**

## Discussion

This method results in an document state refresh with an invocation to: -\[BETextInput requestTextContextForAutocorrectionWithCompletionHandler:\]

## See Also

### Text selection

func selectionWillChange(for: any BETextInput)

Tells the system when the selection is about to change in the document.

**Required**

