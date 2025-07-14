

- ProximityReader
- PaymentCardReaderSession
-  PaymentCardReaderSession.ReadError 

Enumeration

# PaymentCardReaderSession.ReadError

Errors that can occur during a card read.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
enum ReadError
```

## Mentioned in 

Accepting loyalty passes from Wallet

Adding support for Tap to Pay on iPhone to your app

## Topics

### Getting the error

case cardReadFailed

An error occurred when reading the card.

case invalidAmount

The request contained an invalid amount.

case invalidCurrencyCode

The request included an invalid currency code.

case invalidPreferredAID

The preferred AID specified in the transaction request is invalid.

case invalidVASMerchants(String?)

The specified list of VAS merchants list is invalid.

case invalidVASRequestParameters(String?)

The specified VAS parameters are invalid.

case nfcDisabled

NFC is disabled on the device.

case noReaderSession

No reader session available or the session isn’t ready.

case passcodeDisabled

Read operations aren’t allowed when the device’s passcode is disabled.

case paymentCardDeclined

The payment card declined the transaction.

case paymentReadFailed

An internal failure prevented the read operation.

case pinCancelled

The current PIN capture was cancelled, also cancelling any ongoing read operation.

case pinNotAllowed

The time window allowed for a PIN capture after a card read has expired or requesting the PIN is simply not supported by your current configuration.

case pinEntryFailed

An error occurred when capturing the PIN.

case pinEntryTimeout

The current PIN capture was not completed in allowed time.

case pinTokenInvalid

An error that indicates an invalid PIN token.

case readCancelled

The current read operation was cancelled.

case readFromBackgroundError

Read operations aren’t allowed when an app is in the background state.

case readNotAllowed

The read operation isn’t allowed at this time.

case readNotAllowedDuringCall

Read operations aren’t allowed during a phone call.

case readerServiceConnectionError

The session wasn’t able to connect the system UI or other services.

case readerServiceError

A general reader service internal state issue occurred.

case readerSessionAuthenticationError

An authentication error occurred while refreshing the reader session.

case readerSessionBusy

The reader is busy with another session.

case readerSessionExpired

The reader session expired and couldn’t refresh due to other state changes.

case readerSessionNetworkError

A network error occurred that prevented a reader session refresh.

case readerTokenExpired

The configuration token for the reader session expired.

case vasReadFail

An error occurred when reading a loyalty pass.

### Describing the error

var errorDescription: String

A description of the error in plain text.

var errorName: String

### Enumeration Cases

case storeAndForwardDeclineFailed

Decline request was made after the allowance time window.

case storeAndForwardResultNotFound

Decline request failed because the framework can’t find the read result.

case unknown(code: Int)

An unexpected error happened, try again.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- Error
- Sendable

