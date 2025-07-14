

- App Intents
- AppIntent
-  requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:) 

Instance Method

# requestConfirmation(conditions:actionName:dialog:showDialogAsPrompt:content:)

Request user confirmation before performing the app intent.

AppIntentsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func requestConfirmation(
    conditions: ConfirmationConditions = [],
    actionName: ConfirmationActionName = .`continue`,
    dialog: IntentDialog? = nil,
    showDialogAsPrompt: Bool = true,
    @ViewBuilder content: () -> Content
) async throws where Content : View
```

## Parameters 

`conditions`  

The preconditions for requesting confirmation.

`actionName`  

The name for the confirmation action.

`dialog`  

The confirmation dialog.

`showDialogAsPrompt`  

Flag indicating whether the confirmation dialog should be displayed as prompt text with the confirmation.

`content`  

The `View` to display for confirmation.

## See Also

### Requesting confirmation

func requestConfirmation() async throws

Requests user confirmation before performing the app intent.

func requestConfirmation(conditions: ConfirmationConditions, actionName: ConfirmationActionName, dialog: IntentDialog) async throws

Requests user confirmation before performing the app intent.

func requestConfirmation&lt;Result>(result: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throws

Requests user confirmation before performing the app intent.

Deprecated

func requestConfirmation&lt;Result>(output: Result, confirmationActionName: ConfirmationActionName, showPrompt: Bool) async throwsDeprecated

