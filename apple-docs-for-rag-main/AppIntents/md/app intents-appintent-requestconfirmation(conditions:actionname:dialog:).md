

- App Intents
- AppIntent
-  requestConfirmation(conditions:actionName:dialog:) 

Instance Method

# requestConfirmation(conditions:actionName:dialog:)

Requests user confirmation before performing the app intent.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func requestConfirmation(
    conditions: ConfirmationConditions = [],
    actionName: ConfirmationActionName = .`continue`,
    dialog: IntentDialog
) async throws
```

## Parameters 

`conditions`  

The preconditions for requesting confirmation.

`actionName`  

The name for the confirmation action.

`dialog`  

The confirmation dialog.

## See Also

### Requesting confirmation

func requestConfirmation() async throws

Requests user confirmation before performing the app intent.

func requestConfirmation&lt;Content>(conditions: ConfirmationConditions, actionName: ConfirmationActionName, dialog: IntentDialog?, showDialogAsPrompt: Bool, content: () -> Content) async throws

Request user confirmation before performing the app intent.

func requestConfirmation&lt;Result>(result: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throws

Requests user confirmation before performing the app intent.

Deprecated

func requestConfirmation&lt;Result>(output: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throwsDeprecated

