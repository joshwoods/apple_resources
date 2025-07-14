

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  dismiss(completion:) 

Instance Method

# dismiss(completion:)

Dismisses the payment sheet.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
func dismiss(completion: (() -> Void)? = nil)
```

``` source
func dismiss() async
```

## Parameters 

`completion`  

A block that is called after the sheet is dismissed.

## Discussion

Call this method when you receive the paymentAuthorizationControllerDidFinish(_:) delegate callback, or otherwise want to dismiss the payment sheet.

## See Also

### Handling user interactions

var delegate: (any PKPaymentAuthorizationControllerDelegate)?

The controller’s delegate.

protocol PKPaymentAuthorizationControllerDelegate

Methods that let you respond to user interactions with your payment authorization controller.

func present(completion: ((Bool) -> Void)?)

Presents the payment sheet modally over your app.

