

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  init(paymentRequest:) 

Initializer

# init(paymentRequest:)

Initializes and returns a payment authorization view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
init?(paymentRequest request: PKPaymentRequest)
```

## Parameters 

`request`  

The payment request to be authorized.

## Return Value

The newly initialized view controller.

## Discussion

If the user can’t make payments on any of the payment request’s supported networks, initialization fails and this method returns `nil`.

Present and dismiss the view controller using the appropriate mechanism and style for the current device idiom.

## See Also

### Creating a payment authorization view controller

convenience init(disbursementRequest: PKDisbursementRequest)

Initializes and returns a new payment authorization view controller with the provided disbursement request.

