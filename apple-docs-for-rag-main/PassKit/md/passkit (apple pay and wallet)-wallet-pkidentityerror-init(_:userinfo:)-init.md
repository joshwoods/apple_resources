

- PassKit (Apple Pay and Wallet)
- Wallet
- PKIdentityError
-  init(\_:userInfo:) 

Initializer

# init(\_:userInfo:)

Creates an identity error with an error code and user information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 2.0+Xcode 7.2+

``` source
init(
    _ code: Code,
    userInfo: [String : Any] = [:]
)
```

## Parameters 

`code`  

The error code.

`userInfo`  

The user info to associate with the error.

