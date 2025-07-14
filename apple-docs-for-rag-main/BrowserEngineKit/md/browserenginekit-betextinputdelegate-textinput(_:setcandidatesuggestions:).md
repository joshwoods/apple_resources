

- BrowserEngineKit
- BETextInputDelegate
-  textInput(\_:setCandidateSuggestions:) 

Instance Method

# textInput(\_:setCandidateSuggestions:)

Provides text suggestions to the system.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
func textInput(
    _ textInput: any BETextInput,
    setCandidateSuggestions suggestions: [BETextSuggestion]?
)
```

**Required**

## Discussion

For example, suggestions could include data list elements or AutoFill candidates.

