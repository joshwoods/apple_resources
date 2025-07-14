

- StoreKit
- PaymentMethodBinding
- PaymentMethodBinding.PaymentMethodBindingError
-  PaymentMethodBinding.PaymentMethodBindingError.failed 

Case

# PaymentMethodBinding.PaymentMethodBindingError.failed

The initialization or binding operation failed.

iOS 16.4+iPadOS 16.4+visionOS 1.0+

``` source
case failed
```

## Discussion

The methods of the PaymentMethodBinding struct can fail if the app isn’t entitled to use this API, or if other errors occur.

## See Also

### Getting error codes

case invalidPinningID

The in-app binding identifier is invalid or expired.

case notEligible

The user isn’t eligible.

