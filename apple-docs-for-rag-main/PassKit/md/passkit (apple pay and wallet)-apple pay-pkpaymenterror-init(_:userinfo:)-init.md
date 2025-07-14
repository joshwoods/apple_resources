

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKPaymentError
-  init(\_:userInfo:) 

Initializer

# init(\_:userInfo:)

Creates a payment error object of the specified type with the specified user information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
init(
    _ code: Code,
    userInfo: [String : Any] = [:]
)
```

## Parameters 

`code`  

The error code for the type of payment error.

`userInfo`  

The additional details for the error.

