

- Core Telephony
-  CTSubscriber 

Class

# CTSubscriber

A cellular network subscriber.

iOS 7.0+iPadOS 7.0+

``` source
class CTSubscriber
```

## Topics

### Identifying the subscriber

var identifier: String

An implementation-defined identifier used to correlate this subscriber with information vended by other APIs.

### Working with a delegate

var delegate: (any CTSubscriberDelegate)?

A delegate that receives updates on the subscriber information.

### Managing the carrier token

var carrierToken: Data?

A data object containing authorization information about the subscriber.

func refreshCarrierToken() -> Bool

Attempts to refresh the carrier token.

let CTSubscriberTokenRefreshed: String

The name of the notification indicating that the carrier token is available.

Deprecated

### Detecting a SIM

var isSIMInserted: Bool

A Boolean property that indicates whether a SIM is present.

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

### Subscriber Information

protocol CTSubscriberDelegate

A protocol to handle changes to subscriber information.

class CTSubscriberInfo

An object that provides an array of cellular network subscribers.

