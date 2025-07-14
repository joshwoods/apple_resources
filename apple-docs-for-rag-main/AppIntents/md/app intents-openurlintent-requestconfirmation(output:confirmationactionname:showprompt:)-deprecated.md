

- App Intents
- OpenURLIntent
-  requestConfirmation(output:confirmationActionName:showPrompt:) Deprecated

Instance Method

# requestConfirmation(output:confirmationActionName:showPrompt:)

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+Mac Catalyst 16.0+

``` source
func requestConfirmation(
    output: Result,
    confirmationActionName: ConfirmationActionName = .`continue`,
    showPrompt: Bool = true
) async throws where Result : IntentResult
```

Deprecated

Please use requestConfirmation(conditions:actionName:dialog:) or requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:)

