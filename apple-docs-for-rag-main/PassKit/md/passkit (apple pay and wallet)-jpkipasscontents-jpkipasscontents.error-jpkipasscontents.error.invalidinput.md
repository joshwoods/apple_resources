

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Error
-  JPKIPassContents.Error.invalidInput 

Case

# JPKIPassContents.Error.invalidInput

The PIN or password doesn’t meet the specified conditions.

iOS 18.0+iPadOS 18.0+

``` source
case invalidInput
```

## Discussion

This error occurs when there’s an attempt to update the PIN or password for a digitial identity and the provided information doesn’t meet the defined requirements.

## See Also

### Error cases

case appNotForeground

The calling app isn’t in the foreground.

case biometricUnavailable

Biometric authorization isn’t available.

Deprecated

case incorrectUserAuthentication

The provided credential authentication request wasn’t accepted.

Deprecated

case resourceNotAvailable

The system resouce is currently unavailable.

