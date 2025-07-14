

- BrowserEngineKit
- BETextInputDelegate
-  textInput(\_:deferReplaceTextActionToSystem:) 

Instance Method

# textInput(\_:deferReplaceTextActionToSystem:)

Defers a replace text action to the ssytem.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
func textInput(
    _ textInput: any BETextInput,
    deferReplaceTextActionToSystem sender: Any
)
```

**Required**

## Discussion

When handling the replace: action, use this method to defer the replacement to the system.

For example, a replacement could be deferred after it is selected from the autocorrect replacements list.

## See Also

### Deferring actions to the text system

func shouldDeferEventHandlingToSystem(for: any BETextInput, context: BEKeyEntryContext) -> Bool

Defers the key event to the system and returns whether the key event was handled.

**Required**

