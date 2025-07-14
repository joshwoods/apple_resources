

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Error
-  JPKIPassContents.Error.userAuthenticationFailed(remainingRetryAttempts:) 

Case

# JPKIPassContents.Error.userAuthenticationFailed(remainingRetryAttempts:)

Credential authentication request provided was rejected.

iOS 18.4+iPadOS 18.4+

``` source
case userAuthenticationFailed(remainingRetryAttempts: Int)
```

## Discussion

- remainingRetryAttempts: The number of failed attempts left before the credential is locked out.

