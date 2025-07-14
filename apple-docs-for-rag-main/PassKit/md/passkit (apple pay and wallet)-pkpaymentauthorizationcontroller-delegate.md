

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  delegate 

Instance Property

# delegate

The controller’s delegate.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
weak var delegate: (any PKPaymentAuthorizationControllerDelegate)? { get set }
```

## Discussion

The delegate is called at various points in the interaction, such as when the user selects shipping or billing information and when the user authorizes the payment request.

## See Also

### Handling user interactions

protocol PKPaymentAuthorizationControllerDelegate

Methods that let you respond to user interactions with your payment authorization controller.

func present(completion: ((Bool) -> Void)?)

Presents the payment sheet modally over your app.

func dismiss(completion: (() -> Void)?)

Dismisses the payment sheet.

