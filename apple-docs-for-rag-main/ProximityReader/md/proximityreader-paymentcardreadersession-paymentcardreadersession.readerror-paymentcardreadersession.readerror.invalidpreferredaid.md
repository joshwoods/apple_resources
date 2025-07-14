

- ProximityReader
- PaymentCardReaderSession
- PaymentCardReaderSession.ReadError
-  PaymentCardReaderSession.ReadError.invalidPreferredAID 

Case

# PaymentCardReaderSession.ReadError.invalidPreferredAID

The preferred AID specified in the transaction request is invalid.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
case invalidPreferredAID
```

## Discussion

This error occurs when you specify preferred AIDs or RIDs that aren’t between the range of 5 to 16 bytes, or the list has too many entries.

## See Also

### Getting the error

case cardReadFailed

An error occurred when reading the card.

case invalidAmount

The request contained an invalid amount.

case invalidCurrencyCode

The request included an invalid currency code.

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

