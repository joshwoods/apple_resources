

- Messages
- MSMessagesAppViewController
-  didResignActive(with:) 

Instance Method

# didResignActive(with:)

Invoked after the message resigns its active status.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func didResignActive(with conversation: MSConversation)
```

## Parameters 

`conversation`  

The conversation that the user is currently viewing in the Messages app.

## Discussion

Override this method to perform any cleanup activities after the Messages extension has been dismissed. Avoid doing any time-consuming tasks in your implementation.

## See Also

### Managing the Extension’s State

var activeConversation: MSConversation?

The conversation currently displayed in the transcript.

func dismiss()

Dismisses the extension and marks it for termination.

func willBecomeActive(with: MSConversation)

Invoked just before the Messages extension becomes active.

func didBecomeActive(with: MSConversation)

Invoked after the Messages extension becomes active.

func willResignActive(with: MSConversation)

Invoked just before the message resigns its active status.

