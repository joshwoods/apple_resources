

- App Intents
- AppIntent
-  requestConfirmation(output:confirmationActionName:showPrompt:) Deprecated

Instance Method

# requestConfirmation(output:confirmationActionName:showPrompt:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func requestConfirmation(
    output: Result,
    confirmationActionName: ConfirmationActionName = .`continue`,
    showPrompt: Bool = true
) async throws where Result : IntentResult
```

Deprecated

Please use requestConfirmation(conditions:actionName:dialog:) or requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:)

## See Also

### Requesting confirmation

func requestConfirmation() async throws

Requests user confirmation before performing the app intent.

func requestConfirmation(conditions: ConfirmationConditions, actionName: ConfirmationActionName, dialog: IntentDialog) async throws

Requests user confirmation before performing the app intent.

func requestConfirmation&lt;Content>(conditions: ConfirmationConditions, actionName: ConfirmationActionName, dialog: IntentDialog?, showDialogAsPrompt: Bool, content: () -> Content) async throws

Request user confirmation before performing the app intent.

func requestConfirmation&lt;Result>(result: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throws

Requests user confirmation before performing the app intent.

Deprecated

