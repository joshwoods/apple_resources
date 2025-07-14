

- ProximityReader
- PaymentCardReaderError
-  PaymentCardReaderError.accountAlreadyLinked 

Case

# PaymentCardReaderError.accountAlreadyLinked

An error that indicates the merchant already accepted the Terms and Conditions.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
case accountAlreadyLinked
```

## Discussion

The merchant has already accepted the Terms and Conditions. Your app needs to call prepare(using:) to configure the device.

## See Also

### Getting the error code

case accountDeactivated

An error that indicates the linked Apple Account account has been deactivated by the merchant.

case accountLinkingCancelled

An error that indicates the user cancelled the linking or relinking operation.

case accountLinkingCheckFailed

An error that indicates the system couldn’t check the account status of the merchant.

case accountLinkingFailed

An error that indicates the system couldn’t link or relink the merchant using the provided Apple Account.

case accountLinkingRequiresiCloudSignIn

An error that indicates the merchant must be signed into iCloud to accept the Terms and Conditions.

case accountNotLinked

An error that indicates the merchant must accept the Terms and Conditions with a valid Apple Account.

case backgroundRequestNotAllowed

An error that results from requests to the reader while the host app is in the background state.

case deviceBanned(Date?)

An error that indicates the device is banned until the specified date.

case emptyReaderToken

An error that indicates the reader token is empty, which is invalid.

case invalidMerchant

An error that indicates the merchant is invalid or unknown.

case invalidReaderToken(String?)

An error that indicates an invalid, non-empty reader token.

case merchantBlocked

An error that indicates the merchant is blocked.

case modelNotSupported

An error that indicates the current device isn’t supported.

case networkAuthenticationError

An authentication error that occurred during connection to the server.

case networkError

A network error.

