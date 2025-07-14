

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Error
-  JPKIPassContents.Error.biometricUnavailable Deprecated

Case

# JPKIPassContents.Error.biometricUnavailable

Biometric authorization isn’t available.

iOS 18.0–18.4DeprecatediPadOS 18.0–18.4Deprecated

``` source
case biometricUnavailable
```

Deprecated

Use biometricAuthenticationFailed(laError: LocalAuthentication.LAError) instead

## See Also

### Error cases

case appNotForeground

The calling app isn’t in the foreground.

case incorrectUserAuthentication

The provided credential authentication request wasn’t accepted.

Deprecated

case invalidInput

The PIN or password doesn’t meet the specified conditions.

case resourceNotAvailable

The system resouce is currently unavailable.

