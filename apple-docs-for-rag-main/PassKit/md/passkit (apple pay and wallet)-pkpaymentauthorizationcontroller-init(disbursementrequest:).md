

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  init(disbursementRequest:) 

Initializer

# init(disbursementRequest:)

Creates a new payment authorization controller with the disbursement request you provide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
convenience init(disbursementRequest request: PKDisbursementRequest)
```

## Parameters 

`request`  

A PKDisbursementRequest that contains the details of the request.

## See Also

### Creating a payment authorization controller

init(paymentRequest: PKPaymentRequest)

Initializes and returns a payment authorization controller.

