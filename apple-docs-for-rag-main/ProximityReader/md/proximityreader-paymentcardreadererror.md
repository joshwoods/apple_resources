

- ProximityReader
-  PaymentCardReaderError 

Enumeration

# PaymentCardReaderError

An error type that indicates problems with the configuration of the reader.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
enum PaymentCardReaderError
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Topics

### Getting the error code

case accountAlreadyLinked

An error that indicates the merchant already accepted the Terms and Conditions.

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

case notAllowed

An error usually caused by an entitlement issue, an invalid application bundle, a configuration issue, or a token issue.

case notReady

An error that indicates the reader session isn’t ready.

case osVersionNotSupported

An error that indicates the current OS version isn’t supported.

case passcodeDisabled

An error that indicates the device doesn’t have an active passcode.

case prepareExpired

An error that indicates the reader’s session expired.

case prepareFailed(String?)

An error that indicates preparation failed.

case readerBusy

An error that indicates the card reader is busy.

case readerMemoryFull

An error that indicates the reader’s internal memory is full.

case serviceConnectionError

An error that indicates an internal service is unavailable.

case tokenExpired

An error that indicates the reader’s token expired.

case unsupported

An error that indicates unsupported hardware or a problem with the device.

case unknown(code: Int)

An unexpected error happened, try again.

### Getting the error details

var errorDescription: String

A plain-text description of the error.

var errorName: String

The name of the error.

### Enumeration Cases

case storeAndForwardNotAllowed

An error that indicates the framework can’t create a Store and Forward session because:

case storeAndForwardSessionExpired

An error that indicates the framework can’t execute more reads using the current Store and Forward session, because it’s expired.

case storeAndForwardSessionInvalidated

An error that indicates the framework invalidated the current Store and Forward session, and it can’t execute additional reads.

case storeAndForwardTokenIssuerChanged

An error that indicates the current Store and Forward mode has payments from a different token issuer.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- Error
- Sendable

## See Also

### Errors

enum MobileDocumentReaderError

An error type that indicates problems when preparing a mobile document reader session and performing document requests.

