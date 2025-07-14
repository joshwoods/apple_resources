

- Message UI
- MFMessageComposeViewController
-  messageComposeDelegate 

Instance Property

# messageComposeDelegate

The delegate to which message-related notifications should be sent.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var messageComposeDelegate: (any MFMessageComposeViewControllerDelegate)? { get set }
```

## Discussion

When the user taps a button to send or cancel the message, your delegate is notified and should respond by dismissing the message composition interface. For more information about implementing the methods of your delegate object, see MFMessageComposeViewControllerDelegate.

## See Also

### Responding to the view controller dismissal

protocol MFMessageComposeViewControllerDelegate

An interface for responding to user interactions with a message compose view controller.

