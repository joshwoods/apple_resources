

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationResult
-  init(status:errors:) 

Initializer

# init(status:errors:)

Initializes the result with the status code and list of errors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    status: PKPaymentAuthorizationStatus,
    errors: [any Error]?
)
```

## Parameters 

`status`  

The status of the payment.

`errors`  

Any errors returned from the authorization status.

