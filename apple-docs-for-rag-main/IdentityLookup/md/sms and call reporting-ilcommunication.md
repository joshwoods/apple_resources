

- SMS and Call Reporting
-  ILCommunication 

Class

# ILCommunication

An abstract superclass representing a message or call to the user.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILCommunication
```

## Topics

### Accessing Data

var sender: String?

The email address or phone number of the sender.

var dateReceived: Date

The date and time when the system received the message.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ILCallCommunication
- ILMessageCommunication

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

### Communications

class ILMessageCommunication

A concrete subclass representing a SMS message.

class ILCallCommunication

A concrete subclass representing a phone call.

