

- Core NFC
- NFCPresentmentIntentAssertion
-  NFCPresentmentIntentAssertion.Error 

Enumeration

# NFCPresentmentIntentAssertion.Error

An error type that indicates problems with the presentment intent assertion.

iOS 17.4+iPadOS 17.4+

``` source
enum Error
```

## Topics

### Presentment intent assertion errors

case systemEligibilityFailed

The current system isn’t eligible to use this service.

case systemNotAvailable

The system is unavailable because it’s in the cool-down period.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Testing presentment intention validity

var isValid: Bool

A Boolean property that indicates whether the presentment intent assertion instance is still valid.

