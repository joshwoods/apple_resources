

- App Intents
- OpenURLIntent
-  requestConfirmation(result:confirmationActionName:showPrompt:) Deprecated

Instance Method

# requestConfirmation(result:confirmationActionName:showPrompt:)

Requests user confirmation before performing the app intent.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+Mac Catalyst 16.0+

``` source
func requestConfirmation(
    result: Result,
    confirmationActionName: ConfirmationActionName = .`continue`,
    showPrompt: Bool = true
) async throws where Result : IntentResult
```

Deprecated

Please use requestConfirmation(conditions:actionName:dialog:) or requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:)

## Discussion

Use requestConfirmation(conditions:actionName:dialog:) or `requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:)` instead.

