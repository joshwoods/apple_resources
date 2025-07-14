

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  init(disbursementRequest:) 

Initializer

# init(disbursementRequest:)

Initializes and returns a new payment authorization view controller with the provided disbursement request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
convenience init(disbursementRequest request: PKDisbursementRequest)
```

## Parameters 

`request`  

A PKDisbursementRequest.

## See Also

### Creating a payment authorization view controller

init?(paymentRequest: PKPaymentRequest)

Initializes and returns a payment authorization view controller.

