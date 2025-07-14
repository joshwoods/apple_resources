

- BrowserEngineKit
- BETextInputDelegate
-  invalidateTextEntryContext(for:) 

Instance Method

# invalidateTextEntryContext(for:)

Tells the system the text entry context has changed and that text entry UI’s need to be refreshed.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
func invalidateTextEntryContext(for textInput: any BETextInput)
```

**Required**

## Discussion

This is a costly operation and should only used with intention. For example, when switching focus between different elements.

