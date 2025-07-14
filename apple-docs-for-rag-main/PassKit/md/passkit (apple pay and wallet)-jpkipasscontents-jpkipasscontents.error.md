

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.Error 

Enumeration

# JPKIPassContents.Error

Defines a set of possible errors.

iOS 18.0+iPadOS 18.0+

``` source
enum Error
```

## Topics

### Error cases

case appNotForeground

The calling app isn’t in the foreground.

case biometricUnavailable

Biometric authorization isn’t available.

Deprecated

case incorrectUserAuthentication

The provided credential authentication request wasn’t accepted.

Deprecated

case invalidInput

The PIN or password doesn’t meet the specified conditions.

case resourceNotAvailable

The system resouce is currently unavailable.

### Enumeration Cases

case biometricAuthenticationFailed(laError: LAError)

Biometric authorization failed

case unknownError

Unknown error occurred

case userAuthenticationFailed(remainingRetryAttempts: Int)

Credential authentication request provided was rejected.

## Relationships

### Conforms To

- Error
- Sendable

