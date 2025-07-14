

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  init(paymentRequest:) 

Initializer

# init(paymentRequest:)

Initializes and returns a payment authorization controller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
init(paymentRequest request: PKPaymentRequest)
```

## Parameters 

`request`  

The payment request to be authorized.

## Return Value

The newly initialized view controller.

## Discussion

If the user can’t make payments on any of the payment request’s supported networks, initialization fails and this method returns `nil`.

Present and dismiss the controller by calling its present(completion:) and dismiss(completion:) methods.

## See Also

### Creating a payment authorization controller

convenience init(disbursementRequest: PKDisbursementRequest)

Creates a new payment authorization controller with the disbursement request you provide.

