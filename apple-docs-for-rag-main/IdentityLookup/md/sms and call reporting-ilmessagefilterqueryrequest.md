

- SMS and Call Reporting
-  ILMessageFilterQueryRequest 

Class

# ILMessageFilterQueryRequest

A request for a Message Filter app extension to determine the status of a message received from an unknown sender.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILMessageFilterQueryRequest
```

## Topics

### Getting Information About a Message

var sender: String?

The sender of the message.

var messageBody: String?

The body of a message received from an unknown sender.

var receiverISOCountryCode: String?

The ISO Country Code of the receiving phone number, in format specified by the ISO 3166-2 standard.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Queries

protocol ILMessageFilterQueryHandling

A set of methods implemented by a Message Filter app extension to handle query requests.

