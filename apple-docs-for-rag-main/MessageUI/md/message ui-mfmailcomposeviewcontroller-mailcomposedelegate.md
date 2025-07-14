

- Message UI
- MFMailComposeViewController
-  mailComposeDelegate 

Instance Property

# mailComposeDelegate

The mail composition view controller’s delegate.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var mailComposeDelegate: (any MFMailComposeViewControllerDelegate)? { get set }
```

## Discussion

The delegate object is responsible for dismissing the view presented by this view controller at the appropriate time. Therefore, you should always provide a delegate, and that object should implement the methods of the MFMailComposeViewControllerDelegate protocol.

## See Also

### Responding to the view controller dismissal

protocol MFMailComposeViewControllerDelegate

An interface for responding to user interactions with a mail compose view controller.

