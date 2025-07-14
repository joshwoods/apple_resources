

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Error
-  JPKIPassContents.Error.biometricAuthenticationFailed(laError:) 

Case

# JPKIPassContents.Error.biometricAuthenticationFailed(laError:)

Biometric authorization failed

iOS 18.4+iPadOS 18.4+

``` source
case biometricAuthenticationFailed(laError: LAError)
```

## Discussion

- laError. LocalAuthentication.LAError issued by the LocalAuthentication framework.

