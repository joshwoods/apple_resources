

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Error
-  JPKIPassContents.Error.incorrectUserAuthentication Deprecated

Case

# JPKIPassContents.Error.incorrectUserAuthentication

The provided credential authentication request wasn’t accepted.

iOS 18.0–18.4DeprecatediPadOS 18.0–18.4Deprecated

``` source
case incorrectUserAuthentication
```

Deprecated

Use userAuthenticationFailed(remainingRetryAttempts: Int) instead

## Discussion

For example, this error occurs if the PIN provided is incorrect.

## See Also

### Error cases

case appNotForeground

The calling app isn’t in the foreground.

case biometricUnavailable

Biometric authorization isn’t available.

Deprecated

case invalidInput

The PIN or password doesn’t meet the specified conditions.

case resourceNotAvailable

The system resouce is currently unavailable.

