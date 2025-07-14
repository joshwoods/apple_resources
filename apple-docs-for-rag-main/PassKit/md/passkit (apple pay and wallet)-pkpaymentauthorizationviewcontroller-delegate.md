

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  delegate 

Instance Property

# delegate

The view controller’s delegate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any PKPaymentAuthorizationViewControllerDelegate)? { get set }
```

## Discussion

The delegate is called at various points in the interaction, such as when the user selects shipping or billing information and when the user authorizes the payment request.

## See Also

### Handling user interactions

protocol PKPaymentAuthorizationViewControllerDelegate

Methods that let you respond to user interactions with your payment authorization view controller.

