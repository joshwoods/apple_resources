

- Messages
- MSMessagesAppViewController
-  dismiss() 

Instance Method

# dismiss()

Dismisses the extension and marks it for termination.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func dismiss()
```

## Discussion

Call this method to dismiss the extension. The system displays the keyboard if there is any content in the Messages app’s input field. If the input field is empty, the system dismisses the keyboard entirely.

This method also marks the extension as eligible for termination, causing the system to call the view controller’s willResignActive(with:) and didResignActive(with:) methods.

## See Also

### Managing the Extension’s State

var activeConversation: MSConversation?

The conversation currently displayed in the transcript.

func willBecomeActive(with: MSConversation)

Invoked just before the Messages extension becomes active.

func didBecomeActive(with: MSConversation)

Invoked after the Messages extension becomes active.

func willResignActive(with: MSConversation)

Invoked just before the message resigns its active status.

func didResignActive(with: MSConversation)

Invoked after the message resigns its active status.

