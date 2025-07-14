

- Messages
- MSMessagesAppViewController
-  activeConversation 

Instance Property

# activeConversation

The conversation currently displayed in the transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
var activeConversation: MSConversation? { get }
```

## Discussion

This is the conversation that the user is currently viewing in the Messages app.

## See Also

### Managing the Extension’s State

func dismiss()

Dismisses the extension and marks it for termination.

func willBecomeActive(with: MSConversation)

Invoked just before the Messages extension becomes active.

func didBecomeActive(with: MSConversation)

Invoked after the Messages extension becomes active.

func willResignActive(with: MSConversation)

Invoked just before the message resigns its active status.

func didResignActive(with: MSConversation)

Invoked after the message resigns its active status.

