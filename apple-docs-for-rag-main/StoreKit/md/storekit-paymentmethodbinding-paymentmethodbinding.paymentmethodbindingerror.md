

- StoreKit
- PaymentMethodBinding
-  PaymentMethodBinding.PaymentMethodBindingError 

Enumeration

# PaymentMethodBinding.PaymentMethodBindingError

Error information for payment method binding.

iOS 16.4+iPadOS 16.4+visionOS 1.0+

``` source
enum PaymentMethodBindingError
```

## Overview

The methods of PaymentMethodBinding may return these errors, as well as the StoreKitError.userCancelled error.

## Topics

### Getting error codes

case failed

The initialization or binding operation failed.

case invalidPinningID

The in-app binding identifier is invalid or expired.

case notEligible

The user isn’t eligible.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

