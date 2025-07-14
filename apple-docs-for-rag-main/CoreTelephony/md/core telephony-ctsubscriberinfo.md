

- Core Telephony
-  CTSubscriberInfo 

Class

# CTSubscriberInfo

An object that provides an array of cellular network subscribers.

iOS 6.0+iPadOS 6.0+

``` source
class CTSubscriberInfo
```

## Overview

Use the CTSubscriber instances provided by this class to identify individual subscribers by their carrierToken or identifier properties.

## Topics

### Getting Subscriber Information

class func subscribers() -> [CTSubscriber]

Returns the cellular network subscribers.

class func subscriber() -> CTSubscriber

Returns the cellular network subscribers.

Deprecated

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

class CTSubscriber

A cellular network subscriber.

protocol CTSubscriberDelegate

A protocol to handle changes to subscriber information.

