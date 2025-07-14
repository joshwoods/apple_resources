

- Messages
- MSMessagesAppViewController
-  willResignActive(with:) 

Instance Method

# willResignActive(with:)

Invoked just before the message resigns its active status.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func willResignActive(with conversation: MSConversation)
```

## Parameters 

`conversation`  

The conversation that the user is currently viewing in the Messages app.

## Discussion

Override this method to perform any cleanup activities just before the Messages extension is dismissed. Avoid doing any time-consuming tasks in your implementation. This method should return as quickly as possible. Also, avoid making asynchronous calls, because the extension might terminate before the asynchronous tasks have completed.

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

func didResignActive(with: MSConversation)

Invoked after the message resigns its active status.

