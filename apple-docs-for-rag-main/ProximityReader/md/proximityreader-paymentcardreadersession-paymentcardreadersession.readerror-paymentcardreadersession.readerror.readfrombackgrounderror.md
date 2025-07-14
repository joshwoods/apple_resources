

- ProximityReader
- PaymentCardReaderSession
- PaymentCardReaderSession.ReadError
-  PaymentCardReaderSession.ReadError.readFromBackgroundError 

Case

# PaymentCardReaderSession.ReadError.readFromBackgroundError

Read operations aren’t allowed when an app is in the background state.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
case readFromBackgroundError
```

## See Also

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

