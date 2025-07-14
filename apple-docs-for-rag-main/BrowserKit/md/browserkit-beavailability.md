

- BrowserKit
-  BEAvailability 

Class

# BEAvailability

A class that tests whether a device is eligible to run an alternative browser engine.

iOS 18.4+iPadOS 18.4+

``` source
class BEAvailability
```

## Topics

### Testing eligibility

class func isEligible(for: BEAvailability.Context, completionHandler: (Bool, (any Error)?) -> Void)

Tests whether the device is eligible to use an app that contains an alternative browser engine.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Testing eligibility to use alternative browser engines

enum Context

The category of app for which you determine eligibility.

