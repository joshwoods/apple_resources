

- Core NFC
- NFCPresentmentIntentAssertion
- NFCPresentmentIntentAssertion.Error
-  NFCPresentmentIntentAssertion.Error.systemNotAvailable 

Case

# NFCPresentmentIntentAssertion.Error.systemNotAvailable

The system is unavailable because it’s in the cool-down period.

iOS 17.4+iPadOS 17.4+

``` source
case systemNotAvailable
```

## Discussion

CoreNFC enforces a cool-down period after one NFCPresentmentIntentAssertion invalidates and before you can acquire another one. If you receive this error, wait a short time before trying to acquire a new NFCPresentmentIntentAssertion.

## See Also

### Presentment intent assertion errors

case systemEligibilityFailed

The current system isn’t eligible to use this service.

