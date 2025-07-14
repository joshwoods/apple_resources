

- Core NFC
- CardSession
- CardSession.Error
-  CardSession.Error.systemEligibilityFailed 

Case

# CardSession.Error.systemEligibilityFailed

The current system setting or hardware configuation isn’t eligible to use the NFC card emulation service.

iOS 17.4+iPadOS 17.4+

``` source
case systemEligibilityFailed
```

## See Also

### Card session errors

case invalidated

The system invalidated the card session.

case userInvalidated

The person using the app invalidated the card session.

case maxSessionDurationReached

The session is no longer valid because it reached its maximum duration.

case transmissionError

The card session experienced a general error transmitting data.

case systemNotAvailable

A system resource is currently unavailable.

case accessNotAccepted

The person using the app hasn’t yet accepted or declined your app’s request to use the NFC card emulation service.

case emulationStopped

The card emulation stopped.

case radioDisabled

The card session failed because the NFC radio is disabled.

