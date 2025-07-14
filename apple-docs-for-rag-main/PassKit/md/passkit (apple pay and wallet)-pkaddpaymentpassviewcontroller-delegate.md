

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassViewController
-  delegate 

Instance Property

# delegate

The object that acts as the delegate for the add payment view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any PKAddPaymentPassViewControllerDelegate)? { get set }
```

## See Also

### Working with add payment view controllers

protocol PKAddPaymentPassViewControllerDelegate

Methods that let the system prompt you for an add payment request, and inform you when a request has succeeded or failed.

