

- Messages
- MSMessagesAppViewController
-  didBecomeActive(with:) 

Instance Method

# didBecomeActive(with:)

Invoked after the Messages extension becomes active.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func didBecomeActive(with conversation: MSConversation)
```

## Parameters 

`conversation`  

The conversation that the user is currently viewing in the Messages app.

## Discussion

Override this method to respond after the Messages extension becomes active. The extension becomes active both when the user selects the extension from the app drawer, and when the user selects a message in the transcript that represents an MSMessage object created by a copy of the extension.

## See Also

### Managing the Extension’s State

var activeConversation: MSConversation?

The conversation currently displayed in the transcript.

func dismiss()

Dismisses the extension and marks it for termination.

func willBecomeActive(with: MSConversation)

Invoked just before the Messages extension becomes active.

func willResignActive(with: MSConversation)

Invoked just before the message resigns its active status.

func didResignActive(with: MSConversation)

Invoked after the message resigns its active status.

