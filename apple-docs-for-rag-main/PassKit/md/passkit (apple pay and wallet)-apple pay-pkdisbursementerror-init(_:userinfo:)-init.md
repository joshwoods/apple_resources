

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKDisbursementError
-  init(\_:userInfo:) 

Initializer

# init(\_:userInfo:)

Creates a new error structure with the error code and user info you provide.

iOS 8.0+iPadOS 8.0+Mac Catalyst 17.0+macOS 10.10+visionOS 1.0+Xcode 6.0.1+

``` source
init(
    _ code: Code,
    userInfo: [String : Any] = [:]
)
```

## Parameters 

`code`  

A PKDisbursementError.Code that describes the error.

`userInfo`  

Additional information you provide with more details about the specific error condition.

